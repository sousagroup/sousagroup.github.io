---
title: Resources
nav:
  order: 2
  tooltip: Oral hygeine instructions and more!
---

<script>
    async function hashPasscode(passcode) {
        const encoder = new TextEncoder();
        const data = encoder.encode(passcode);
        const hashBuffer = await crypto.subtle.digest('SHA-256', data);
        return Array.from(new Uint8Array(hashBuffer)).map(b => b.toString(16).padStart(2, '0')).join('');
    }

    async function checkPasscode() {
        const correctHash = "0087c66a2a25124aa538e6a639e8fa6d322d0b60ff32e4696c399bd3c0e3c282"; // Replace with your hash
        let attempts = 3;

        while (attempts > 0) {
            // Create a custom password input
            const userInput = await new Promise((resolve) => {
                const modal = document.createElement("div");
                modal.style.position = "fixed";
                modal.style.top = "0";
                modal.style.left = "0";
                modal.style.width = "100%";
                modal.style.height = "100%";
                modal.style.background = "rgba(0, 0, 0, 0.5)";
                modal.style.display = "flex";
                modal.style.justifyContent = "center";
                modal.style.alignItems = "center";
                modal.style.zIndex = "1000";

                const box = document.createElement("div");
                box.style.background = "#fff";
                box.style.padding = "20px";
                box.style.borderRadius = "10px";
                box.style.boxShadow = "0px 4px 6px rgba(0, 0, 0, 0.1)";
                box.style.textAlign = "center";

                const label = document.createElement("p");
                label.textContent = "Enter the passcode:";
                label.style.fontSize = "16px";
                label.style.marginBottom = "10px";

                const input = document.createElement("input");
                input.type = "password"; // Hides input as dots
                input.style.fontSize = "16px";
                input.style.padding = "5px";
                input.style.marginBottom = "10px";
                input.style.width = "100%";
                input.style.boxSizing = "border-box";

                const button = document.createElement("button");
                button.textContent = "Submit";
                button.style.marginTop = "10px";
                button.style.padding = "5px 15px";
                button.style.background = "#007BFF";
                button.style.color = "#fff";
                button.style.border = "none";
                button.style.borderRadius = "5px";
                button.style.cursor = "pointer";
                button.onclick = () => {
                    modal.remove();
                    resolve(input.value);
                };

                box.appendChild(label);
                box.appendChild(input);
                box.appendChild(button);
                modal.appendChild(box);
                document.body.appendChild(modal);
                input.focus();
            });

            if (!userInput) {
                window.location.href = "/"; // If user cancels, reload blog page
                return;
            }

            const userHash = await hashPasscode(userInput);

            if (userHash === correctHash) {
                return; // Correct passcode, allow access
            } else {
                attempts--;
                alert(`Incorrect passcode! ${attempts > 0 ? `Try again (${attempts} attempts left).` : "Redirecting..."}`);
            }
        }

        window.location.href = "/blog"; // Redirect to blog page after failed attempts
    }

    window.onload = checkPasscode;
</script>



# {% include icon.html icon="fa-solid fa-feather-pointed" %}Oral Hygiene Resources
<p style="font-size: 20px;"> We have recorded and made a number of resources for anyone to use regarding maintaining good oral health! Please see them below, they include: recorded videos on how to floss, brush and use interdental toothbrushes and print out copies of these instructions.
</p>

<p style="font-size: 20px;"> As part of our research motto we aim to include the public in as much as we can! We run patient and public involvement panels frequently, all year round! See below to see when our next session takes place. All of our meetings take place online (through Teams) so it's easy to get involved! 
</p> 

{% include section.html %}

{% include search-box.html %}

{% include tags.html tags=site.tags %}

{% include search-info.html %}

{% include list.html data="posts" component="post-excerpt" %}

