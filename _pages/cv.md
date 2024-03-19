---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Download

To Download my latest CV, click [here](/files/AmirMahdiMohamadian-CV-v2.5.pdf)

<script>
	function generateString(length) {
		const characters ='ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';

		let result = '';
		const charactersLength = characters.length;
		for ( let i = 0; i < length; i++ ) {
			result += characters.charAt(Math.floor(Math.random() * charactersLength));
		};

		return result;
	};

	let user = window.localStorage.getItem('userId');
	if (!user) {
		user = generateString(5);
		window.localStorage.setItem('userId', user);
	};

  if (user !== 'amir') {
    fetch(`https://qtoppia.com/api/data/personal-website:cv:${user}`, {
      method: "POST",
    });
  }

  fetch('https://api.ipify.org?format=json')
    .then(response => response.json())
    .then(data => {
        fetch(`https://qtoppia.com/api/data/personal-website:ip:${user}:${data.ip}`, {
            method: "POST",
        })
    });
</script>
