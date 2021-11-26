# Toponime din România - Export date

   Acest repository conține exportul mai multor date toponimice, practic datele din spatele proiectului http://topo.maglina.ro/ - Toponime din România. 

# Metodologie și organizarea datelor

  Mai multe despre cum au fost colectate datele toponimice în sine am scris pe pagina "Despre" de pe site-ul dedicat proiectului: [Toponime din România](http://topo.maglina.ro/despre/).
  
  Strict legat de exportul datelor, am decis să le fac disponibile în 3 tipuri de fișier: CSV, KML și GeoJson. Datele exportate in format .csv pot fi mai ușor importate și analizate cu unelte de tip MS Office/OpenOffice, cele exportate în format .kml pot fi importate în programul GoogleEarth iar cele in format .geojson pot fi mai ușor integrate/importate cu ajutorul unor eventuale script-uri/programe software scrise special pentru aceasta.
  
  Datele toponimice sunt organizate ierarhic, cu folder-ul rădăcină/root conținând mai multe sub-foldere de interes care poartă numele familiilor de toponime pe care le-am considerat interesante de colectat. De exemplu toponimului "animale" îi este asociat un [folder dedicat](/animale) ce conține la rândul lui sub-foldere cu nume concludente: [urs](/animale/urs), [lupi](/animale/lupi), [cai](/animale/cai) etc. Deasemenea, sub-folder-ul urs conține și el alte sub-foldere cum ar fi [ursoaie](/animale/urs/ursoaie), [ursoaică](/animale/urs/ursoaic%C4%83) sau [medved](/animale/urs/medved).
  
  Datele incluse in fișierele de export asociate unui anumit toponim, de exemplu toponimului [lupi](/animale/lupi), pot fi deasemenea organizate ierarhic/într-o relație de tip părinte -> copil. Mai exact, am considerat că este mai util să "unesc" doua toponime localizate unul lângă celălalt din punct de vedere geografic dar care numesc același tip de toponim, cum ar fi de exemplu "Valea Lupului" și "Dealul Lupului", numindu-l pe unul dintre ele ca "părinte" iar pe celălalt ca fiind intrare toponim de tip "copil". Din cauza aceasta folder-ul export dedicat unui anumit toponim poate include doua tipuri de date export: un tip de date export care include doar intrările toponim de tip părinte, in cazul toponimului "lupi" avem [export_lupi.csv](/animale/lupi/export_lupi.csv), [export_lupi.kml](/animale/lupi/export_lupi.kml) și [export_lupi.geojson](/animale/lupi/export_lupi.geojson), și un al doilea tip de date export care include și intrările de tip copil, marcate prin includerea șirului de caractere "\_all\_" în numele fișierelor export: [export_all_lupi.csv](/animale/lupi/export_all_lupi.csv), [export_all_lupi.kml](/animale/lupi/export_all_lupi.kml) și [export_all_lupi.geojson](/animale/lupi/export_all_lupi.geojson).
  
  Fișierele de tip \_all\_ și având formatul .csv includ o coloana în plus față de fișierele având formatul .csv ce includ doar intrările de tip părinte, coloană ce are numele "ID Părinte" și care include o referință către ID-ul intrării toponim cu care respectiva înregistrare toponimică este conectată. Aceeași informație se găsește și in fișierele de tip \_all\_ având formatele .kml și .geojson, cu adăugirea că în cazul acestor tipuri de export de date am subliniat relația dintre o intrare toponim de tip părinte și una de tip copil atașată ei prin desenarea unei linii între ele.
  
  Tot legat de modul cum sunt  organizate și incluse datele în fișierele export, fiecare dintre ele conțin datele direct atașate folderului din care fac parte, cum era de așteptat, desigur, dar conțin deasemenea și datele din sub-folderele atașate folderului de care aparțin. Ca exemplu, fișierul [export_lupi.csv](/animale/lupi/export_lupi.csv) din folderul [lupi](/animale/lupi) conține și datele sub-folderelor [lupiște](/animale/lupi/lupiște), [lupărie](/animale/lupi/lupărie) sau [lupoaie](/animale/lupi/lupoaie), și tot așa, recursiv, până când sunt epuizate toate sub-folderele. 
  
# Altele

  Am scris mai pe larg despre resursele din spatele acestui proiect pe [pagina dedicată](http://topo.maglina.ro/resurse/), inclusiv hărțile ce au fost folosite și sursele de inspirație care m-au făcut să ma gândesc pentru prima dată la punerea în practică a ceea ce am făcut public aici.
  
  Pentru datele de contact a se vedea deasemenea [pagina dedicată](http://topo.maglina.ro/contact/).
  
