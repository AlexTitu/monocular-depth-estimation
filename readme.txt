Proiect: High Quality Monocular Depth Estimation
Autori: Octavian-Florin Marica, Alex-Costin Tițu, Vlad-Eugen Vlăsceanu

Instrucțiuni: 
1. Se descarcă setul de date NYU Depth v2 de la linkul următor: https://www.kaggle.com/datasets/soumikrakshit/nyu-depth-v2
2. Se instalează pachetele: NumPy, torch si torchvision cu cuda, torchmetrics, matplotlib, pandas si PIL
3. Pentru antrenare, se rulează pana la celula cu antetul Training Loop. Pentru a relua antrenarea in cazul unei intreruperi, se foloseste calea folderului unde se salvează dictionarele de stare, cale salvata in variabila „models_dir”, si se decomenteaza toate liniile pentru incarcarea modelului, optimizatorului si a lr_scheduler. De asemenea, se incarca variabila H, variabila istoric (en. History) ce pastreaza progresul functiei de cost in timpul antrenarii pe cele doua seturi.
4. Pentru partea de test, se ruleaza doar celula ce este destinata trasarii graficului curbei functiei de cost si bucla de calcul a metricilor de evaluare pe setul de test (inclus si nu omis din ppt).
5. In final, se pot face cateva inferente prin retea si extrage rezultatele plus imaginile RGB și adâncimile originale apelând penultima bulcă, pentru setul de test și ultima buclă pentru setul de date de evaluare.

Restul comentariilor incluse in cod ar trebui sa explice mai detaliat ce face fiecare functie in parte sau de ce au fost incluse anumite bucati de cod.