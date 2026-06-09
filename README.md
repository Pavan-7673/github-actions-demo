# github-actions-demo
name: CI Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Build
        run: echo "Building the app..."

      - name: Test
        run: echo "Running tests..."

      - name: Deploy
        run: echo "Deploying the app..."
