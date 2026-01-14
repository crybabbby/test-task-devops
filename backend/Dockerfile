FROM python:3.12-slim
WORKDIR /app
RUN groupadd -r appgroup && useradd -r -g appgroup -u 1000 appuser
COPY webapp.py .
RUN chown -R appuser:appgroup /app
USER appuser
EXPOSE 8080
CMD ["python3", "webapp.py"]
