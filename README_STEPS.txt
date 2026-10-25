SADNAN HOSTING  -  Full Credit: Sadnan Codex
=============================================

LOGIN INFO
----------
Login page : /login
Username   : admin
Password   : admin123
(Online dile age password change koro: app.py te "admin123" search kore bodle nao)


A) NIJER PC / TERMUX E RUN (TEST)
---------------------------------
1. Zip extract koro
2. Terminal e folder e jao
3. pip install -r requirements.txt
4. python app.py
5. Browser: http://localhost:5000


B) RENDER E ONLINE (FREE)
-------------------------
1. github.com e new repo banao
2. Zip extract kore SOB file upload koro
   (app.py, requirements.txt, Procfile, html file gulo -> sob repo-r ROOT e, kono folder lagbe na)
3. render.com -> New -> Web Service -> repo connect koro
4. Settings:
     Language       : Python 3
     Build Command  : pip install -r requirements.txt
     Start Command  : gunicorn app:app --bind 0.0.0.0:$PORT --workers 1 --threads 4 --timeout 120
5. Create Web Service -> deploy hoye gele link e jao
6. /login e giye admin / admin123 diye ghuko, tarpor password change koro


NOTE
----
- Workers 1 rakhbe, nahole bot gulo duplicate/kaj korbe na.
- Free Render restart hole bots/ ar users.json muche jete pare.
- Error hole Render er Logs er shesh line pathao.
