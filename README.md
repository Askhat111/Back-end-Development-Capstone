# Back-end Capstone: Django

This repository contains the full application source in `source.zip`, with its original directories, tests, templates and assets preserved. Extract with `python -m zipfile -e source.zip .` to inspect or run the source locally.

The root Dockerfile extracts this same source archive during the build. Build using `docker build -t capstone-django .`.

The implementation builds on the IBM Developer Skills Network course starter. Original license notices are preserved. CRUD, validation and error handling were completed for the capstone.

Testing recorded locally: Pictures 11 supplied pytest tests passed; Songs 4 tests passed against mongomock (a test double, not a live MongoDB server); Django 4 functional tests passed. Cloud deployment evidence is tracked separately and is not claimed by these local test results.

Configuration: Songs reads MONGODB_URI. Django reads SONGS_API_URL, PICTURES_API_URL, DJANGO_ALLOWED_HOSTS and DJANGO_SECRET_KEY. Do not commit credentials. No default administrator credentials are provided.
