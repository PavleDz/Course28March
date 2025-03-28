# Course28March
Test solutions and examples from the mentor session - python day 2 - 28/03/2025

Objašnjenje pristupa u radu drugog zadatka - skrepovanje realitica.com:

Nakon pokušaja da se preko requests modula skrepuje stranica, nastao je problem jer podaci za listing nijesu mogli da se skrepuju. Ranije sam se sretao sa sličnim problemom prilikom scapping-a, i ovo su bili najčešći razlozi:
1. backendu treba header ili cookies u requestu - pokušao sam da kloniram u potpunosti request koji se šalje backend kada se stranica otvori i nije išlo.
2. Postavljene su neke vrste anti-scrappinga.
Ranije sam se susretao sa sličnim problemom i u 90% slučajeva je rješenje otvaranje browsera preko seleniuma i injekcija fetch requesta preko njega - nakon čega se response vraća u python i dalje obrađuje. To sam uradio i u ovom slučaju.
