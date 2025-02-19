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
        let attempts = 3; // Allow multiple tries

        while (attempts > 0) {
            const userInput = prompt("Enter the passcode:");
            if (userInput === null) {
                window.location.href = "/blog"; // If user cancels, reload blog page
                return;
            }

            const userHash = await hashPasscode(userInput);

            if (userHash === correctHash) {
                return; // Correct passcode, allow access
            } else {
                attempts--;
                alert(`Incorrect passcode! ${attempts > 0 ? `Try again!).` : "Redirecting..."}`);
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

