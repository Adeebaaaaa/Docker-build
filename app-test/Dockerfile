# node-service/Dockerfile

FROM node:20-alpine

WORKDIR /app

# Create simple Node script (single line, no quoting problems)
RUN printf 'console.log("Running on architecture:", process.arch); setInterval(() => {}, 100000);\n' > app.js

EXPOSE 3000

CMD ["node", "app.js"]