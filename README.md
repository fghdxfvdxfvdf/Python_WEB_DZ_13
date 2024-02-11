docker-compose up
docker-compose up -d


alembic init migrations

alembic revision --autogenerate -m 'Init'

alembic upgrade head



uvicorn main:app --reload
python -m uvicorn main:app --host localhost --port 8000 --reload


http://localhost:8000/docs
