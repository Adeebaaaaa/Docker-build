# python-service/Dockerfile

FROM python:3.11-alpine

WORKDIR /app

# Create a simple Python file (single line, no quoting issues)
RUN echo 'import http.server, socketserver; print("Running on Python"); socketserver.TCPServer(("", 8080), http.server.SimpleHTTPRequestHandler).serve_forever()' > app.py

EXPOSE 8080

CMD ["python", "app.py"]