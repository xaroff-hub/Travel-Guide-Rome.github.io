# Travel-Guide-Rome.github.io
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Roma Insider</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{--bg:#faf5ee;--card:#fff;--ink:#2a1f1a;--mute:#6f625a;--brand:#b5472a;--brand2:#8f3720;--gold:#c99a3b;--line:#eadfd1;--soft:#f3e8d9;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#1a1411;--card:#241c17;--ink:#f4ebe1;--mute:#b3a496;--brand:#e0714f;--brand2:#c95b3a;--gold:#e0b25a;--line:#3a2e26;--soft:#2d231d}}
:root[data-theme="dark"]{--bg:#1a1411;--card:#241c17;--ink:#f4ebe1;--mute:#b3a496;--brand:#e0714f;--brand2:#c95b3a;--gold:#e0b25a;--line:#3a2e26;--soft:#2d231d}
*{box-sizing:border-box}
html{scroll-behavior:smooth;scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--ink);font-family:Inter,system-ui,-apple-system,Segoe UI,sans-serif;line-height:1.6}
h1,h2,h3{font-family:"Playfair Display",Georgia,serif;line-height:1.15;margin:0}
a{color:inherit}
.wrap{max-width:1040px;margin:0 auto;padding:0 20px}
nav{display:flex;justify-content:space-between;align-items:center;padding:18px 0;gap:10px;flex-wrap:wrap}
.logo{font-family:"Playfair Display",Georgia,serif;font-weight:700;font-size:1.3rem;text-decoration:none}
.logo span{color:var(--brand)}
.right{display:flex;align-items:center;gap:12px}
.langs{display:flex;border:1.5px solid var(--line);border-radius:999px;overflow:hidden}
.langs button{background:transparent;border:0;color:var(--mute);font:600 .8rem Inter,sans-serif;padding:8px 12px;cursor:pointer}
.langs button[aria-pressed="true"]{background:var(--brand);color:#fff}
.btn{display:inline-block;background:var(--brand);color:#fff;border:0;padding:14px 26px;border-radius:999px;font:600 1rem Inter,sans-serif;cursor:pointer;text-decoration:none;text-align:center;transition:.2s}
.btn:hover{background:var(--brand2);transform:translateY(-1px)}
.btn.ghost{background:transparent;color:var(--ink);border:1.5px solid var(--line)}
.btn.ghost:hover{background:var(--soft)}
.btn.sm{padding:9px 18px;font-size:.9rem}
.hero{display:grid;grid-template-columns:1.1fr .9fr;gap:40px;align-items:center;padding:30px 0 70px}
.tag{display:inline-block;background:var(--soft);color:var(--brand);font-weight:600;font-size:.82rem;padding:6px 14px;border-radius:999px;margin-bottom:18px}
.hero h1{font-size:clamp(2.2rem,5vw,3.6rem);margin-bottom:18px}
.hero h1 em{color:var(--brand);font-style:italic}
.hero p{color:var(--mute);font-size:1.1rem;max-width:520px}
.cta{display:flex;gap:12px;flex-wrap:wrap;margin:26px 0 14px}
.proof{font-size:.9rem;color:var(--mute)}
.cover{background:linear-gradient(160deg,var(--brand),#7a2e1a);border-radius:20px;color:#fff;padding:34px 28px;aspect-ratio:3/4;max-width:340px;margin:0 auto;display:flex;flex-direction:column;justify-content:space-between;box-shadow:0 24px 50px rgba(120,50,20,.3);transform:rotate(2deg)}
.cover small{letter-spacing:.2em;text-transform:uppercase;opacity:.8}
.cover h2{font-size:2.4rem}
.cover svg{width:100%;height:90px}
section{padding:60px 0}
.title{text-align:center;margin-bottom:36px}
.title h2{font-size:clamp(1.7rem,4vw,2.4rem);margin-bottom:10px}
.title p{color:var(--mute);margin:0}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:18px}
.card{background:var(--card);border:1px solid var(--line);border-radius:16px;padding:24px}
.card .ic{font-size:1.8rem;margin-bottom:10px}
.card h3{font-size:1.2rem;margin-bottom:6px}
.card p{margin:0;color:var(--mute);font-size:.95rem}
.band{background:var(--soft)}
.tabs{display:flex;gap:8px;justify-content:center;margin-bottom:22px;flex-wrap:wrap}
.tab{border:1.5px solid var(--line);background:var(--card);color:var(--ink);padding:10px 20px;border-radius:999px;font:500 .95rem Inter,sans-serif;cursor:pointer}
.tab[aria-selected="true"]{background:var(--brand);border-color:var(--brand);color:#fff}
.day{background:var(--card);border:1px solid var(--line);border-radius:16px;padding:24px;max-width:720px;margin:0 auto}
.day ol{list-style:none;margin:0;padding:0}
.day li{display:flex;gap:16px;padding:12px 0;border-bottom:1px dashed var(--line)}
.day li:last-child{border:0}
.day b{color:var(--brand);min-width:56px}
.day span{color:var(--mute);font-size:.92rem;display:block}
.lock{text-align:center;color:var(--mute);font-size:.9rem;margin-top:16px}
.plans{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:22px;max-width:760px;margin:0 auto}
.plan{background:var(--card);border:1.5px solid var(--line);border-radius:20px;padding:30px;position:relative;display:flex;flex-direction:column}
.plan.pop{border-color:var(--brand);box-shadow:0 12px 34px rgba(181,71,42,.18)}
.badge{position:absolute;top:-13px;left:50%;transform:translateX(-50%);background:var(--gold);color:#2a1f1a;font-weight:700;font-size:.75rem;padding:5px 14px;border-radius:999px;white-space:nowrap}
.plan h3{font-size:1.4rem}
.price{font:700 2.8rem "Playfair Display",Georgia,serif;margin:10px 0}
.plan ul{list-style:none;padding:0;margin:0 0 24px;flex:1}
.plan li{padding:6px 0 6px 26px;position:relative;font-size:.95rem}
.plan li:before{content:"✓";position:absolute;left:0;color:var(--brand);font-weight:700}
.plan .btn{width:100%}
.guarantee{text-align:center;color:var(--mute);font-size:.9rem;margin-top:24px}
details{background:var(--card);border:1px solid var(--line);border-radius:12px;padding:16px 20px;max-width:720px;margin:0 auto 10px}
summary{cursor:pointer;font-weight:600}
details p{color:var(--mute);margin:10px 0 0}
footer{padding:36px 0;text-align:center;color:var(--mute);font-size:.88rem;border-top:1px solid var(--line)}
.modal{position:fixed;inset:0;background:rgba(0,0,0,.55);display:none;align-items:center;justify-content:center;padding:20px;z-index:10}
.modal.open{display:flex}
.box{background:var(--card);border-radius:20px;padding:30px;max-width:420px;width:100%}
.box h3{margin-bottom:8px}
.box p{color:var(--mute);font-size:.95rem}
.sum{display:flex;justify-content:space-between;font-weight:600;padding:12px 0;border-top:1px solid var(--line);margin:14px 0}
.box .btn{width:100%;display:block}
.box .btn+.btn{margin-top:8px}
@media(max-width:760px){.hero{grid-template-columns:1fr;text-align:center}.hero p{margin:0 auto}.cta{justify-content:center}.cover{order:-1;max-width:240px}}
</style>
</head>
<body>
<div class="wrap">
<nav><a class="logo" href="#">Roma<span>Insider</span></a>
<div class="right"><div class="langs" id="langs"></div><a class="btn sm" id="navbuy" href="#offres"></a></div></nav>
<header class="hero">
<div>
<span class="tag" id="tag"></span>
<h1 id="h1"></h1>
<p id="hp"></p>
<div class="cta"><a class="btn" id="c1" href="#offres"></a><a class="btn ghost" id="c2" href="#apercu"></a></div>
<div class="proof" id="proof"></div>
</div>
<div class="cover">
<small id="cv1"></small>
<svg viewBox="0 0 300 90" fill="none" stroke="currentColor" stroke-width="2" opacity=".85"><path d="M10 80h280M30 80V40a20 20 0 0140 0v40M90 80V40a20 20 0 0140 0v40M150 80V40a20 20 0 0140 0v40M210 80V40a20 20 0 0140 0v40M20 28h250"/></svg>
<div><h2>Rome<br>Insider</h2><small id="cv3"></small></div>
</div>
</header>
</div>

<section><div class="wrap">
<div class="title"><h2 id="ft"></h2><p id="fp"></p></div>
<div class="grid" id="fg"></div>
</div></section>

<section class="band" id="apercu"><div class="wrap">
<div class="title"><h2 id="at"></h2><p id="ap"></p></div>
<div class="tabs" id="tabs" role="tablist"></div>
<div class="day"><ol id="day"></ol></div>
<p class="lock" id="lock"></p>
</div></section>

<section id="offres"><div class="wrap">
<div class="title"><h2 id="ot"></h2><p id="op"></p></div>
<div class="plans" id="plans"></div>
<p class="guarantee" id="guar"></p>
</div></section>

<section class="band"><div class="wrap">
<div class="title"><h2 id="qt"></h2></div>
<div id="faq"></div>
</div></section>

<footer><div class="wrap" id="foot"></div></footer>

<div class="modal" id="modal" role="dialog" aria-modal="true">
<div class="box">
<h3 id="mt"></h3><p id="mp"></p>
<div class="sum"><span id="pn"></span><span id="pp"></span></div>
<a class="btn" id="pay" href="#" target="_blank" rel="noopener"></a>
<button class="btn ghost" id="close"></button>
</div>
</div>

<script>
const PAYPAL="https://paypal.me/lucasslgd/";
const P={ess:9.9,full:19.9};
const L={
fr:{n:"Français",
 tag:"🇮🇹 Guide numérique · Mis à jour 2026",h1:"Visitez Rome <em>comme un local</em>, sans les files d’attente.",
 hp:"Itinéraires jour par jour, bonnes adresses vérifiées, astuces pour éviter les pièges à touristes. Tout ce qu’il faut pour un séjour réussi, dans votre poche.",
 buy:"Acheter",c1:"Obtenir le guide – dès {p}",c2:"Voir un aperçu",proof:"★★★★★ Téléchargement immédiat · Paiement sécurisé PayPal",
 cv1:"Guide de voyage",cv3:"3 jours · 40 adresses",
 ft:"Ce que vous trouverez dedans",fp:"Un guide pensé pour gagner du temps et profiter de chaque heure.",
 f:[["🗺️","3 itinéraires prêts à l’emploi","Rome classique, Rome secrète et Rome en famille, optimisés heure par heure."],["🎟️","Billets et réservations","Colisée, Vatican, Borghèse : quand réserver, où et à quel prix."],["🍝","40 adresses où manger","Trattorias authentiques, meilleurs gelati, pizza al taglio."],["🚇","Transports malins","Métro, bus, tram, taxis officiels et trajets depuis l’aéroport."],["💶","Budget et astuces","Combien prévoir par jour, pourboires, eau gratuite, pièges à éviter."],["📱","Lisible hors ligne","PDF optimisé mobile avec liens Google Maps cliquables."]],
 at:"Un aperçu de l’itinéraire",ap:"Voici comment sont organisées les journées dans le guide.",tabs:["Jour 1 · Antique","Jour 2 · Vatican","Jour 3 · Centre"],
 d:[[["8h30","Colisée, Forum et Palatin","Entrée coupe-file, ordre de visite optimal"],["12h30","Déjeuner à Monti","Trattoria locale hors circuit touristique"],["15h","Capitole et Bocca della Verità","Panorama et pause gelato"],["19h","Aperitivo au Trastevere","Les adresses où l’on mange vraiment bien"]],
 [["8h","Musées du Vatican","Créneau idéal pour éviter les foules"],["11h30","Basilique Saint-Pierre","Dôme, code vestimentaire, sécurité"],["14h","Déjeuner à Prati","Pizza al taglio et trattorias du quartier"],["17h","Château Saint-Ange","Coucher de soleil sur le Tibre"]],
 [["9h","Panthéon et Piazza Navona","Réservation et horaires conseillés"],["12h","Fontaine de Trevi","Le bon moment pour y aller sans cohue"],["15h","Place d’Espagne et Villa Borghèse","Balade, vue et détente"],["20h","Dîner romain traditionnel","Carbonara, cacio e pepe et amatriciana"]]],
 lock:"🔒 Horaires précis, adresses et astuces complètes réservés au guide.",
 ot:"Choisissez votre formule",op:"Paiement unique, sans abonnement.",
 pl:[{n:"Essentiel",l:["Guide PDF complet (60 pages)","3 itinéraires de 1 à 3 jours","20 adresses où manger","Mises à jour gratuites 1 an"],b:"Acheter l’Essentiel"},{n:"Complet",pop:"LE PLUS CHOISI",l:["Tout l’Essentiel","40 adresses + bons plans cachés","Carte interactive Google Maps","Audioguide MP3 des grands sites","Checklist de voyage imprimable"],b:"Acheter le Complet"}],
 guar:"✅ Satisfait ou remboursé 14 jours · 🔐 Paiement sécurisé PayPal · ⚡ Guide envoyé par e-mail après paiement",
 qt:"Questions fréquentes",
 q:[["Comment je reçois le guide ?","Après réception de votre paiement PayPal, le guide vous est envoyé par e-mail à l’adresse de votre compte PayPal."],["Puis-je l’utiliser sans connexion à Internet ?","Oui, le PDF se lit hors ligne. Seuls les liens vers les cartes nécessitent une connexion."],["Les informations sont-elles à jour ?","Le guide est révisé chaque année (horaires, tarifs, règles d’accès) et les mises à jour sont incluses."],["Et si le guide ne me convient pas ?","Vous êtes remboursé dans les 14 jours sur simple demande par e-mail."]],
 foot:"© 2026 RomaInsider · Mentions légales · CGV",
 mt:"Finaliser la commande",mp:"Vous allez être redirigé vers PayPal pour régler en toute sécurité. Le guide vous sera envoyé par e-mail.",pay:"Payer avec PayPal",cl:"Annuler"},
en:{n:"English",
 tag:"🇮🇹 Digital guide · Updated 2026",h1:"Visit Rome <em>like a local</em>, without the queues.",
 hp:"Day-by-day itineraries, verified addresses and tips to dodge tourist traps. Everything you need for a great trip, right in your pocket.",
 buy:"Buy",c1:"Get the guide – from {p}",c2:"See a preview",proof:"★★★★★ Instant delivery · Secure PayPal payment",
 cv1:"Travel guide",cv3:"3 days · 40 spots",
 ft:"What’s inside",fp:"A guide designed to save you time and make the most of every hour.",
 f:[["🗺️","3 ready-to-use itineraries","Classic Rome, hidden Rome and Rome with kids, optimized hour by hour."],["🎟️","Tickets and bookings","Colosseum, Vatican, Borghese: when to book, where and for how much."],["🍝","40 places to eat","Authentic trattorias, the best gelato, pizza al taglio."],["🚇","Smart transport","Metro, buses, trams, official taxis and airport transfers."],["💶","Budget and tips","Daily costs, tipping, free drinking water, scams to avoid."],["📱","Works offline","Mobile-friendly PDF with clickable Google Maps links."]],
 at:"A preview of the itinerary",ap:"Here is how each day is organized in the guide.",tabs:["Day 1 · Ancient","Day 2 · Vatican","Day 3 · Centre"],
 d:[[["8:30","Colosseum, Forum and Palatine","Skip-the-line entry, best visiting order"],["12:30","Lunch in Monti","Local trattoria off the tourist trail"],["3 pm","Capitoline Hill and Mouth of Truth","Panorama and a gelato break"],["7 pm","Aperitivo in Trastevere","Where locals really eat well"]],
 [["8:00","Vatican Museums","Best time slot to avoid the crowds"],["11:30","St. Peter’s Basilica","Dome, dress code, security"],["2 pm","Lunch in Prati","Pizza al taglio and neighbourhood trattorias"],["5 pm","Castel Sant’Angelo","Sunset over the Tiber"]],
 [["9:00","Pantheon and Piazza Navona","Booking and recommended hours"],["12:00","Trevi Fountain","The right time to go without the crush"],["3 pm","Spanish Steps and Villa Borghese","Stroll, views and relaxation"],["8 pm","Traditional Roman dinner","Carbonara, cacio e pepe and amatriciana"]]],
 lock:"🔒 Exact times, addresses and full tips are reserved for the guide.",
 ot:"Choose your plan",op:"One-time payment, no subscription.",
 pl:[{n:"Essential",l:["Full PDF guide (60 pages)","3 itineraries from 1 to 3 days","20 places to eat","Free updates for 1 year"],b:"Buy Essential"},{n:"Complete",pop:"MOST POPULAR",l:["Everything in Essential","40 places + hidden gems","Interactive Google Maps map","MP3 audio guide of the main sights","Printable travel checklist"],b:"Buy Complete"}],
 guar:"✅ 14-day money-back guarantee · 🔐 Secure PayPal payment · ⚡ Guide sent by e-mail after payment",
 qt:"Frequently asked questions",
 q:[["How do I receive the guide?","Once your PayPal payment is received, the guide is sent by e-mail to your PayPal account address."],["Can I use it without an Internet connection?","Yes, the PDF can be read offline. Only the map links need a connection."],["Is the information up to date?","The guide is revised every year (hours, prices, access rules) and updates are included."],["What if I don’t like it?","You get a refund within 14 days on simple request by e-mail."]],
 foot:"© 2026 RomaInsider · Legal notice · Terms of sale",
 mt:"Complete your order",mp:"You will be redirected to PayPal to pay securely. The guide will be sent to you by e-mail.",pay:"Pay with PayPal",cl:"Cancel"},
de:{n:"Deutsch",
 tag:"🇮🇹 Digitaler Reiseführer · Stand 2026",h1:"Entdecken Sie Rom <em>wie ein Einheimischer</em> – ohne Schlange stehen.",
 hp:"Tagespläne, geprüfte Adressen und Tipps, um Touristenfallen zu umgehen. Alles für eine gelungene Reise, direkt in Ihrer Tasche.",
 buy:"Kaufen",c1:"Reiseführer holen – ab {p}",c2:"Vorschau ansehen",proof:"★★★★★ Sofortige Lieferung · Sichere PayPal-Zahlung",
 cv1:"Reiseführer",cv3:"3 Tage · 40 Adressen",
 ft:"Das erwartet Sie",fp:"Ein Reiseführer, der Zeit spart und jede Stunde optimal nutzt.",
 f:[["🗺️","3 fertige Routen","Klassisches Rom, geheimes Rom und Rom mit Kindern, Stunde für Stunde geplant."],["🎟️","Tickets und Reservierungen","Kolosseum, Vatikan, Borghese: wann, wo und zu welchem Preis buchen."],["🍝","40 Adressen zum Essen","Echte Trattorien, das beste Eis, Pizza al taglio."],["🚇","Clever unterwegs","Metro, Bus, Tram, offizielle Taxis und Flughafentransfer."],["💶","Budget und Tipps","Tageskosten, Trinkgeld, Trinkwasser, Abzocke vermeiden."],["📱","Offline lesbar","Mobiloptimiertes PDF mit anklickbaren Google-Maps-Links."]],
 at:"Vorschau auf die Route",ap:"So sind die Tage im Reiseführer aufgebaut.",tabs:["Tag 1 · Antike","Tag 2 · Vatikan","Tag 3 · Zentrum"],
 d:[[["8:30","Kolosseum, Forum und Palatin","Eintritt ohne Anstehen, beste Besuchsreihenfolge"],["12:30","Mittagessen in Monti","Lokale Trattoria abseits der Touristenpfade"],["15:00","Kapitol und Bocca della Verità","Panorama und Eispause"],["19:00","Aperitivo in Trastevere","Wo Einheimische wirklich gut essen"]],
 [["8:00","Vatikanische Museen","Beste Zeit, um dem Andrang zu entgehen"],["11:30","Petersdom","Kuppel, Kleiderordnung, Sicherheit"],["14:00","Mittagessen in Prati","Pizza al taglio und Trattorien im Viertel"],["17:00","Engelsburg","Sonnenuntergang über dem Tiber"]],
 [["9:00","Pantheon und Piazza Navona","Reservierung und empfohlene Zeiten"],["12:00","Trevi-Brunnen","Der richtige Zeitpunkt ohne Gedränge"],["15:00","Spanische Treppe und Villa Borghese","Spaziergang, Aussicht und Entspannung"],["20:00","Traditionelles römisches Abendessen","Carbonara, Cacio e Pepe und Amatriciana"]]],
 lock:"🔒 Genaue Zeiten, Adressen und alle Tipps sind dem Reiseführer vorbehalten.",
 ot:"Wählen Sie Ihr Paket",op:"Einmalzahlung, kein Abo.",
 pl:[{n:"Basis",l:["Kompletter PDF-Reiseführer (60 Seiten)","3 Routen von 1 bis 3 Tagen","20 Adressen zum Essen","1 Jahr kostenlose Updates"],b:"Basis kaufen"},{n:"Komplett",pop:"AM BELIEBTESTEN",l:["Alles aus Basis","40 Adressen + Geheimtipps","Interaktive Google-Maps-Karte","MP3-Audioguide der Hauptsehenswürdigkeiten","Druckbare Reise-Checkliste"],b:"Komplett kaufen"}],
 guar:"✅ 14 Tage Geld-zurück-Garantie · 🔐 Sichere PayPal-Zahlung · ⚡ Versand per E-Mail nach Zahlung",
 qt:"Häufige Fragen",
 q:[["Wie erhalte ich den Reiseführer?","Nach Eingang Ihrer PayPal-Zahlung senden wir ihn per E-Mail an die Adresse Ihres PayPal-Kontos."],["Kann ich ihn ohne Internet nutzen?","Ja, das PDF ist offline lesbar. Nur die Kartenlinks benötigen eine Verbindung."],["Sind die Informationen aktuell?","Der Reiseführer wird jährlich überarbeitet (Zeiten, Preise, Zugangsregeln), Updates sind inklusive."],["Was, wenn er mir nicht gefällt?","Sie erhalten innerhalb von 14 Tagen auf formlose E-Mail Ihr Geld zurück."]],
 foot:"© 2026 RomaInsider · Impressum · AGB",
 mt:"Bestellung abschließen",mp:"Sie werden zu PayPal weitergeleitet, um sicher zu bezahlen. Der Reiseführer wird Ihnen per E-Mail gesendet.",pay:"Mit PayPal bezahlen",cl:"Abbrechen"},
it:{n:"Italiano",
 tag:"🇮🇹 Guida digitale · Aggiornata 2026",h1:"Visita Roma <em>come un romano</em>, senza code.",
 hp:"Itinerari giorno per giorno, indirizzi verificati e consigli per evitare le trappole per turisti. Tutto per un viaggio riuscito, in tasca.",
 buy:"Acquista",c1:"Ottieni la guida – da {p}",c2:"Guarda l’anteprima",proof:"★★★★★ Consegna immediata · Pagamento sicuro con PayPal",
 cv1:"Guida di viaggio",cv3:"3 giorni · 40 indirizzi",
 ft:"Cosa trovi dentro",fp:"Una guida pensata per farti risparmiare tempo e sfruttare ogni ora.",
 f:[["🗺️","3 itinerari pronti all’uso","Roma classica, Roma segreta e Roma con i bambini, ottimizzati ora per ora."],["🎟️","Biglietti e prenotazioni","Colosseo, Vaticano, Borghese: quando prenotare, dove e a che prezzo."],["🍝","40 indirizzi dove mangiare","Trattorie autentiche, i migliori gelati, pizza al taglio."],["🚇","Trasporti intelligenti","Metro, bus, tram, taxi ufficiali e transfer dall’aeroporto."],["💶","Budget e consigli","Spesa giornaliera, mance, acqua gratis, truffe da evitare."],["📱","Leggibile offline","PDF ottimizzato per mobile con link Google Maps cliccabili."]],
 at:"Anteprima dell’itinerario",ap:"Ecco come sono organizzate le giornate nella guida.",tabs:["Giorno 1 · Antica","Giorno 2 · Vaticano","Giorno 3 · Centro"],
 d:[[["8:30","Colosseo, Foro e Palatino","Ingresso salta-fila, ordine di visita ideale"],["12:30","Pranzo a Monti","Trattoria locale fuori dai percorsi turistici"],["15:00","Campidoglio e Bocca della Verità","Panorama e pausa gelato"],["19:00","Aperitivo a Trastevere","Dove i romani mangiano davvero bene"]],
 [["8:00","Musei Vaticani","Fascia oraria ideale per evitare la folla"],["11:30","Basilica di San Pietro","Cupola, abbigliamento, sicurezza"],["14:00","Pranzo a Prati","Pizza al taglio e trattorie del quartiere"],["17:00","Castel Sant’Angelo","Tramonto sul Tevere"]],
 [["9:00","Pantheon e Piazza Navona","Prenotazione e orari consigliati"],["12:00","Fontana di Trevi","Il momento giusto per andare senza ressa"],["15:00","Piazza di Spagna e Villa Borghese","Passeggiata, vista e relax"],["20:00","Cena romana tradizionale","Carbonara, cacio e pepe e amatriciana"]]],
 lock:"🔒 Orari precisi, indirizzi e consigli completi sono riservati alla guida.",
 ot:"Scegli la tua formula",op:"Pagamento unico, senza abbonamento.",
 pl:[{n:"Essenziale",l:["Guida PDF completa (60 pagine)","3 itinerari da 1 a 3 giorni","20 indirizzi dove mangiare","Aggiornamenti gratuiti per 1 anno"],b:"Acquista Essenziale"},{n:"Completa",pop:"LA PIÙ SCELTA",l:["Tutto l’Essenziale","40 indirizzi + dritte nascoste","Mappa interattiva Google Maps","Audioguida MP3 dei principali siti","Checklist di viaggio stampabile"],b:"Acquista Completa"}],
 guar:"✅ Soddisfatti o rimborsati 14 giorni · 🔐 Pagamento sicuro PayPal · ⚡ Guida inviata via e-mail dopo il pagamento",
 qt:"Domande frequenti",
 q:[["Come ricevo la guida?","Dopo aver ricevuto il pagamento PayPal, la guida ti viene inviata via e-mail all’indirizzo del tuo account PayPal."],["Posso usarla senza connessione a Internet?","Sì, il PDF si legge offline. Solo i link alle mappe richiedono la connessione."],["Le informazioni sono aggiornate?","La guida viene rivista ogni anno (orari, prezzi, regole di accesso) e gli aggiornamenti sono inclusi."],["E se la guida non mi piace?","Vieni rimborsato entro 14 giorni con una semplice richiesta via e-mail."]],
 foot:"© 2026 RomaInsider · Note legali · Condizioni di vendita",
 mt:"Completa l’ordine",mp:"Verrai reindirizzato a PayPal per pagare in sicurezza. La guida ti sarà inviata via e-mail.",pay:"Paga con PayPal",cl:"Annulla"}
};
const $=id=>document.getElementById(id);
let lang="fr",dayI=0,plan=null;
const money=n=>n.toLocaleString(lang,{style:"currency",currency:"EUR"});
function render(){
const t=L[lang];document.documentElement.lang=lang;
$("langs").innerHTML=Object.keys(L).map(k=>`<button data-l="${k}" aria-pressed="${k==lang}" title="${L[k].n}">${k.toUpperCase()}</button>`).join("");
$("navbuy").textContent=t.buy;$("tag").textContent=t.tag;$("h1").innerHTML=t.h1;$("hp").textContent=t.hp;
$("c1").textContent=t.c1.replace("{p}",money(P.ess));$("c2").textContent=t.c2;$("proof").textContent=t.proof;
$("cv1").textContent=t.cv1;$("cv3").textContent=t.cv3;
$("ft").textContent=t.ft;$("fp").textContent=t.fp;
$("fg").innerHTML=t.f.map(f=>`<div class="card"><div class="ic">${f[0]}</div><h3>${f[1]}</h3><p>${f[2]}</p></div>`).join("");
$("at").textContent=t.at;$("ap").textContent=t.ap;$("lock").textContent=t.lock;
$("tabs").innerHTML=t.tabs.map((x,i)=>`<button class="tab" role="tab" data-d="${i}" aria-selected="${i==dayI}">${x}</button>`).join("");
$("day").innerHTML=t.d[dayI].map(s=>`<li><b>${s[0]}</b><div>${s[1]}<span>${s[2]}</span></div></li>`).join("");
$("ot").textContent=t.ot;$("op").textContent=t.op;
$("plans").innerHTML=t.pl.map((p,i)=>{const k=i?"full":"ess";return `<div class="plan${p.pop?" pop":""}">${p.pop?`<span class="badge">${p.pop}</span>`:""}<h3>${p.n}</h3><div class="price">${money(P[k])}</div><ul>${p.l.map(x=>`<li>${x}</li>`).join("")}</ul><button class="btn${p.pop?"":" ghost"}" data-p="${i}">${p.b}</button></div>`}).join("");
$("guar").textContent=t.guar;$("qt").textContent=t.qt;
$("faq").innerHTML=t.q.map(q=>`<details><summary>${q[0]}</summary><p>${q[1]}</p></details>`).join("");
$("foot").textContent=t.foot;
$("mt").textContent=t.mt;$("mp").textContent=t.mp;$("pay").textContent=t.pay;$("close").textContent=t.cl;
if(plan!==null)fillModal();
}
function fillModal(){const k=plan?"full":"ess";$("pn").textContent=L[lang].pl[plan].n;$("pp").textContent=money(P[k]);$("pay").href=PAYPAL+P[k].toFixed(2)+"EUR"}
function setLang(l){lang=l;try{localStorage.setItem("lang",l)}catch(e){}render()}
document.addEventListener("click",e=>{
const b=e.target.closest("button");if(!b)return;
if(b.dataset.l)setLang(b.dataset.l);
else if(b.dataset.d){dayI=+b.dataset.d;render()}
else if(b.dataset.p){plan=+b.dataset.p;fillModal();$("modal").classList.add("open")}
else if(b.id=="close"){$("modal").classList.remove("open")}
});
$("modal").onclick=e=>{if(e.target.id=="modal")$("modal").classList.remove("open")};
let saved=null;try{saved=localStorage.getItem("lang")}catch(e){}
const nav=(navigator.language||"fr").slice(0,2);
lang=L[saved]?saved:(L[nav]?nav:"fr");
render();
</script>
</body>
</html>
