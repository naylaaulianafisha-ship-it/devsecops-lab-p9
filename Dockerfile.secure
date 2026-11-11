FROM python:3.12-alpine
RUN addgroup -g 1001 -S appgroup && adduser -u 1001 -S appuser -G appgroup
WORKDIR /app
COPY --chown=appuser:appgroup app.py .
USER appuser
EXPOSE 8000
CMD ["python", "app.py"]
