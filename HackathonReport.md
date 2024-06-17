# HackathonReport
Report for our Hackathon Experience at Eth Global Brussels from 12th-14th of July.

## Team && Roles
- **Paul Grossmann (pgrossma)**: Frontend, Backend && Database
- **Louen Greau (lgreau)**: Blockchain Connection && Backend
- **Leon Zipp (lzipp)**: Backend, Database && Blockchain Connection

## Project: Address Relation Visualizer for Ethereum-Blockchain
The goal of our project was to write a simple program that could do the following:
1. Ask for a public address.
2. Scan the ethereum blockchain for every transaction related to this public address.
3. Save the resulting transactions & other relevant data to the database
4. Visualize the corresponding relations.
5. Make resulting data downloadable as csv, xlsx, etc.

### Technologies
#### Backend
- **Go**: Golang was used to create the backend and establish the connection to the ethereum network. For code creation we used...
  - **go-ethereum**: We used this library to connect our backend to the ethereum blockchain. For this we created an eth-client instance, wrapped it in a helper-struct and implemented methods for this struct to run all necessary functionalities.
  - **sqlc**: This library helps converting (postgre)sql code to go code, making it injection-proof while doing so. It saves a lot of work, because instead of writing pure go, we could instead write much simpler & shorter sql-statements instead.
#### Database
- **SQL (Postgresql)**: Our database was written using postgres. The structure can be seen here: [image]...
#### Hosting
- **Docker**:
  - **docker images**:
    - **Backend**: We wrote our own docker image from the base go-image.
    - **Database**: For this we used the standard postgres docker image. 
  - **docker-compose**: Since we only had 48 hours & none of us are well-versed in kubernetes, we decided on using docker-compose instead. Even though it is less safe & stable compared to kubernetes, it is easy to use and can be quickly set up.
  - **devcontainer**: For not having to run every command using docker-compose, we chose to use a devcontainer in conjunction with vscode. As the image the dev-stage of our backend image was used.
#### Authentication
- **keycloak**

## 12th of July
Lorem markdownum pisces [quicquam generumque](http://magni.com/) sequantur tam
talis umero, per. Struxisse quod digna, est [et
aere](http://turres.net/orienteunica) dum. Bracchia inopino correpti Venere face
frenato; valebam, minitantiaque *sustinet lux*; omnem, veluti Eurytidae adhuc;
liber. Tibi Pittheia naides ut quis tempestivus erat, auxilium discumbere mihi,
quod omni. Fortis cannas, quisquis ad arduus mansit: audet socios saevis.

> Terrae nec pro perfundere glaebas rauco; [amore
> tanta](http://licet-tunc.com/facto.html), et illo, madefactis armarat. Amnem
> fata parat. Dum sic enim nunc sucos et fatis generis, herbas mea: verba
> formaeque somno. Manibus esse ignibus alios stimulosque magno dominos.
> Volucrum ara quicquid est velit mea crescit proprium origo det, harundine
> rapite.

Submittere tamen sidera [fecere](http://www.mollis.net/); illa dixit secreta
formam: opus variari. Velle caesas ripas guttae esse atque, secutum tegebat
aetas pendebant coniunx perdam adflat. E *canis minimum* abrumpit tempora
**temptat animam**, Bubasides aspicit marinae sumptaque capilli, profecti.

1. Talia erat oculis
2. Ethemon ad usus pennas totusque
3. Nunc munere

Submittere tamen sidera [fecere](http://www.mollis.net/); illa dixit secreta
formam: opus variari. Velle caesas ripas guttae esse atque, secutum tegebat
aetas pendebant coniunx perdam adflat. E *canis minimum* abrumpit tempora
**temptat animam**, Bubasides aspicit marinae sumptaque capilli, profecti.


- Talia erat oculis
- Ethemon ad usus pennas totusque
- Nunc munere

- ## 13th of July
Lorem markdownum pisces [quicquam generumque](http://magni.com/) sequantur tam
talis umero, per. Struxisse quod digna, est [et
aere](http://turres.net/orienteunica) dum. Bracchia inopino correpti Venere face
frenato; valebam, minitantiaque *sustinet lux*; omnem, veluti Eurytidae adhuc;
liber. Tibi Pittheia naides ut quis tempestivus erat, auxilium discumbere mihi,
quod omni. Fortis cannas, quisquis ad arduus mansit: audet socios saevis.

> Terrae nec pro perfundere glaebas rauco; [amore
> tanta](http://licet-tunc.com/facto.html), et illo, madefactis armarat. Amnem
> fata parat. Dum sic enim nunc sucos et fatis generis, herbas mea: verba
> formaeque somno. Manibus esse ignibus alios stimulosque magno dominos.
> Volucrum ara quicquid est velit mea crescit proprium origo det, harundine
> rapite.

Submittere tamen sidera [fecere](http://www.mollis.net/); illa dixit secreta
formam: opus variari. Velle caesas ripas guttae esse atque, secutum tegebat
aetas pendebant coniunx perdam adflat. E *canis minimum* abrumpit tempora
**temptat animam**, Bubasides aspicit marinae sumptaque capilli, profecti.

1. Talia erat oculis
2. Ethemon ad usus pennas totusque
3. Nunc munere

Submittere tamen sidera [fecere](http://www.mollis.net/); illa dixit secreta
formam: opus variari. Velle caesas ripas guttae esse atque, secutum tegebat
aetas pendebant coniunx perdam adflat. E *canis minimum* abrumpit tempora
**temptat animam**, Bubasides aspicit marinae sumptaque capilli, profecti.


- Talia erat oculis
- Ethemon ad usus pennas totusque
- Nunc munere

- ## 14th of July
Lorem markdownum pisces [quicquam generumque](http://magni.com/) sequantur tam
talis umero, per. Struxisse quod digna, est [et
aere](http://turres.net/orienteunica) dum. Bracchia inopino correpti Venere face
frenato; valebam, minitantiaque *sustinet lux*; omnem, veluti Eurytidae adhuc;
liber. Tibi Pittheia naides ut quis tempestivus erat, auxilium discumbere mihi,
quod omni. Fortis cannas, quisquis ad arduus mansit: audet socios saevis.

> Terrae nec pro perfundere glaebas rauco; [amore
> tanta](http://licet-tunc.com/facto.html), et illo, madefactis armarat. Amnem
> fata parat. Dum sic enim nunc sucos et fatis generis, herbas mea: verba
> formaeque somno. Manibus esse ignibus alios stimulosque magno dominos.
> Volucrum ara quicquid est velit mea crescit proprium origo det, harundine
> rapite.

Submittere tamen sidera [fecere](http://www.mollis.net/); illa dixit secreta
formam: opus variari. Velle caesas ripas guttae esse atque, secutum tegebat
aetas pendebant coniunx perdam adflat. E *canis minimum* abrumpit tempora
**temptat animam**, Bubasides aspicit marinae sumptaque capilli, profecti.

1. Talia erat oculis
2. Ethemon ad usus pennas totusque
3. Nunc munere

Submittere tamen sidera [fecere](http://www.mollis.net/); illa dixit secreta
formam: opus variari. Velle caesas ripas guttae esse atque, secutum tegebat
aetas pendebant coniunx perdam adflat. E *canis minimum* abrumpit tempora
**temptat animam**, Bubasides aspicit marinae sumptaque capilli, profecti.


- Talia erat oculis
- Ethemon ad usus pennas totusque
- Nunc munere
