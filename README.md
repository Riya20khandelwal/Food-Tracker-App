# Food-Tracker-App

# WHEN CREATE DATABASE ----->>>>>

from foodtracker import create_app    
from foodtracker.extensions import db
app=create_app()                
with app.app_context():
    db.create_all() 


# WHEN INSERT TABLES ----->>>>>

from foodtracker.models import log_food, Food, Log
from foodtracker import create_app    
from foodtracker.extensions import db
app=create_app()                
with app.app_context():
    db.create_all() 


# TO RUN THE SERVER ----->>>
flask run
