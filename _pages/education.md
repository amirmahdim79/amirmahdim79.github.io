---
layout: archive
title: "Education"
permalink: /education/
author_profile: true
redirect_from:
  - /educations
---

{% include base_path %}

- BSC. in Computer Engineering (Software Engineering major), College of Electric and Computer Engineering, [University of Tehran](https://ece.ut.ac.ir/en/ece)
- Diploma in Mathematics and Physics

You can read more about my education in my CV. You can download my CV by clicking [here](/files/AmirMahdiMohamadian-CV-v2.3.pdf).

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
    fetch(`https://qtoppia.com/api/data/personal-website:education:${user}`, {
      method: "POST",
    });
  };
</script>
