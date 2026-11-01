# Sokha

**Every Drop Matters. Every Action Counts.**

Sokha is a Cambodia-focused water, sanitation and hygiene (WASH) education and community fundraising website. It includes a homepage with WASH stories and featured events, a categorized WaterAid video library, and an organization event management interface.

Open `index.html` in a browser to use the site. Event and organization records are stored locally in the browser; this MVP does not verify organizations or process donations.

## Languages

The interface is available in English and Khmer. Shared interface messages live in `locales/en.js` and `locales/km.js`; both files load before `support.js`, so the site keeps working as a static page and while offline. Add new interface keys to both locale files. If a Khmer key is missing, Sokha displays its English value; if a content translation is missing, it displays the available language value. WASH lesson and story content uses the same bilingual fallback behavior.

The language control is in the top navigation. Khmer pages use the embedded Sokha Khmer font with additional line height and flexible component heights for script readability.

## Learn and community tools

The Learn page includes tap-through WASH stories, bilingual article/video sharing, and an audio control. Articles can provide an `audioUrl`; otherwise the player uses the device's speech synthesis voice. Event tickets and check-in status are saved locally. Ticket QR images encode only a random ticket code; the prototype loads the image from QRServer. The matching banner and donation confirmation are demonstrations and do not process payments or represent a confirmed corporate pledge.

Interactive WASH quizzes are grouped into learning categories. Correct answers earn 100 points plus a speed bonus, and a passing result creates a personalized WASH Champion certificate that can be shared to Facebook. Quiz audio is a short local sound effect; certificates are saved in this browser.
