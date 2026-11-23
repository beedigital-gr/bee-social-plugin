# BeeDigital Social Offers

Plugin για το ChatGPT. Σου επιτρέπει να διαχειρίζεσαι πελάτες, προσφορές, PIN, κείμενα σελίδας και παραδείγματα από το dashboard https://client.beedigital.gr/_social/ μέσα από συνομιλία.

## Εγκατάσταση

1. Άνοιξε το ChatGPT → Settings → Plugins.
2. Πάτα **Add plugin marketplace**.
3. Βάλε `beedigital-gr/bee-social-plugin`, ref `main`.
4. Εγκατάστησε το **BeeDigital Social Offers**.
5. Συνδέσου με το email και τον κωδικό που χρησιμοποιείς στο dashboard.

## Παραδείγματα

- «Δείξε μου τους πελάτες μου.»
- «Πόσοι άνοιξαν την προσφορά του πελάτη Χ;»
- «Φτιάξε νέα προσφορά για τον πελάτη Χ με αυτό το Canva link.»
- «Άλλαξε τον τίτλο της προσφοράς Υ σε ...»
- «Βγάλε νέο PIN για τον πελάτη Χ.»

## Τι δεν μπορεί να κάνει

Δεν ανεβάζει αρχεία. PDF προσφορές, φωτογραφίες, λογότυπα και νέα παραδείγματα ανεβαίνουν από το dashboard. Το plugin σου δίνει τον σωστό σύνδεσμο.

## Προβλήματα

- Δεν απαντά ή ζητά σύνδεση: συνδέσου ξανά από Settings → Plugins.
- Δεν βρίσκει το marketplace: έλεγξε ότι έγραψες `beedigital-gr/bee-social-plugin` και ref `main`.
- Κάτι άλλο: μίλα με τον Mike.

Για developers: ο τύπος μεταφοράς στο `plugins/bee-social/mcp.json` είναι `streamable-http` (όπως στο portable format). Αν το ChatGPT τον απορρίψει, δοκίμασε `http`.

Σημείωση: το δημοσιευμένο JSON schema του mcp.json δεν δέχεται `extensions` ανά server, αλλά η τεκμηρίωση του OpenAI το ορίζει εκεί για το OAuth. Ακολουθούμε την τεκμηρίωση.
