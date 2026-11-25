

### askel askeleelta: 
Tee Githubiin uusi reposity ja asenna sinne myös README ja GNU3 -tiedostot  

    $ sudo apt-get install git   
    $ git clone https://github.com/VaMaija/GIT-training //kopioi tiedot githubista  
    $ ls //paikalliselle koneelle on ilmestynyt kansio GIT-training
    $ git pull //päivittää reposityn uudet päivitykset koneelle, olin tehnyt tämän ohjetiedoston ohjeet.md joka tuli päivityksenä.  

<img width="350" height="128" alt="Näyttökuva 2026-11-22 203701" src="https://github.com/user-attachments/assets/d9fb89df-80cf-4bf6-8107-6acfb74e4ac6" />  

    $ micro ohjeet.md //tätä käyttämällä pääsen tekemään uutta tekstiä ohjeisiin paikalliselta koneelta. 
    $ git add . //avaa ns näytämön, "haluan näyttää sinulle tekemäni muutokset"
    $ git commit -m "tein ohjetta eteenpäin" //päivittää lokin.  
    $ git push //lähettää päivitetyn tiedoston reposityyn.  

En saanut git pushia toimimaan. Tämä vaati uuden tokenin lisäämisen Githubin kautta.  
1. Settings
2. Vasemmalta täysin alimpana Developer settings
3. Personal Access tokens >> classic
4. Generate new token
5. valitse Classic
6. oikeudeksi "repo"
7. Generate token (ota talteen ja kopio Salasanan kohdalle gitiin kun pyytää salasanaa)

<img width="831" height="344" alt="Näyttökuva 2026-11-22 215715" src="https://github.com/user-attachments/assets/c40cc66a-a721-4e01-b573-943eaad01714" />  

<img width="391" height="115" alt="Näyttökuva 2026-11-22 221134" src="https://github.com/user-attachments/assets/0ba6795a-4ff7-436e-a1a6-da6257ad94b4" />  



1. Lisätään Reposityyn screenshots -kansio:   
    $ mkdir screenshots    
    $ git add .
    $ git commit 
    $ git push    

Jokaisen commitin yhteydessä ei kuitenkaan jaksa etsiä muistiinpanoista tokenia salasanaksi. Lisätään SSH-yhteys: 

    maija@Virtuaali:~/GIT-training$ git remote set-url origin git@github.com:VaMaija/GIT-training.git
    maija@Virtuaali:~/GIT-training$ git remote -v
    origin	git@github.com:VaMaija/GIT-training.git (fetch)
    origin	git@github.com:VaMaija/GIT-training.git (push)

tämän jälkeen ei pitäisi enää kysyä githubin käyttäjänimeä tai tokenia.  








    
