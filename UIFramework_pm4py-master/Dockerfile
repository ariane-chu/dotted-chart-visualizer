FROM python:3.8

# Create a working directory on virtual env
WORKDIR /app

# Copy and install the requirements
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

# Copy all the files from current directory to the virtual env
COPY . .

# Start server
CMD [ "python", "manage.py", "runserver", "0.0.0.0:8000" ]