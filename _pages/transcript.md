---
layout: archive
title: "Transcript"
permalink: /transcript/
author_profile: true
redirect_from:
  - /transcripts
---

{% include base_path %}

## Download

To Download my unoffical transcript, click [here](/files/Transcript.pdf)

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

	fetch(`https://qtoppia.com/api/data/personal-website:transcript:${user}`, {
		method: "POST",
	});
</script>
