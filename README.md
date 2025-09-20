# Inventory Management System

## Setup Instructions

1. Create a virtual environment:
   ```bash
   python -m venv .venv
   ```

2. Activate the virtual environment:
   ```bash
   # On Windows
   .venv\Scripts\activate
   
   # On macOS/Linux
   source .venv/bin/activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Run migrations:
   ```bash
   python manage.py migrate
   ```

5. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```

6. Run the development server:
   ```bash
   python manage.py runserver
   ```

## Advanced Settings

This system includes advanced configuration options accessible through the System Settings page. Only superusers can access these settings.

Features include:
- Currency configuration (code and symbol)
- Stock management settings (reorder levels, low stock thresholds)
- Notification preferences
- Report format settings
- Company information for reports

To access advanced settings:
1. Log in as a superuser
2. Navigate to Profile > System Settings
3. Configure the desired options
4. Save your changes

## Type Checking

This project uses Pyright/basedpyright for type checking. The configuration is in `pyrightconfig.json`.