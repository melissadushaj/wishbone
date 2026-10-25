# Wishbone ꒰ᵕ༚ᵕ⑅꒱ˀˀ 

Make a wish. Keep track of it.

Wishbone is a wishlist app for the things you actually want. Build lists, follow friends, and (coming for the holidays) run a Secret Santa without the group chat chaos.

Built from scratch as a full-stack project. 

![Wishbone profile page](docs/profilepage.png)
## What it does

### Building now

- Accounts with sign up and login
- Wishlists you can name, organize, and fill with wishes (link, price, image, notes)
- A profile page with your lists, followers, and following

### On the wish list

- Follow people and follow individual wishlists
- Public, private, and link-only lists
- **Secret Santa**: create a group, invite people, draw names, and see your match's wishlist (and only theirs)
- A mobile app!
## Tech stack

| Layer | Tools |
| --- | --- |
| Frontend | React, Vite |
| Backend | Django, Django REST Framework |
| Database | SQLite for development, Postgres for production |
| Hosting | Vercel (frontend), TBD (backend) |

## Getting started

You'll need Python 3.14 and Node.js (LTS).

```bash
git clone https://github.com/<your-username>/wishbone.git
cd wishbone
```

### Backend

```bash
cd backend
python3.14 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

The API runs at http://127.0.0.1:8000.

### Frontend


In a second terminal:

```bash
cd frontend
npm install
npm run dev
```

The app runs at http://localhost:5173.

## Project structure

```
wishbone/
├── backend/     # Django project (config/) and apps (users/, ...)
└── frontend/    # React + Vite app
```

## Roadmap

- [x] Django backend and custom user model
- [ ] Wishlist and wish models + API
- [ ] Sign up, log in, log out
- [ ] Profile page connected to real data
- [ ] Privacy settings for lists
- [ ] Follows
- [ ] Secret Santa
- [ ] Deployment

@2026 Melissa ᵕ̈
