FROM apache/airflow:2.9.1-python3.10

# Switch to airflow user BEFORE installing packages
USER airflow

# Copy and install Python dependencies
COPY requirements.txt /requirements.txt
RUN pip install --no-cache-dir -r /requirements.txt
CMD ["airflow", "version"]