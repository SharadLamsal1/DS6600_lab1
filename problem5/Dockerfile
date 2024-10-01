# Use Python 3.11.4 base image
FROM python:3.11.4-bookworm

# Set working directory to /problem5
WORKDIR /problem5

# Copy requirements.txt file to the container
COPY requirements.txt .

# Upgrade pip and install Python dependencies from requirements.txt
RUN pip install --upgrade pip && pip install -r requirements.txt

# Expose port 8888 for JupyterLab
EXPOSE 8888

# Run Jupyter Lab
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--port=8888", "--allow-root"]
