# task3-
name: Test Workflow

on:
  pull_request:
    branches:
      - main

jobs:
  test_job:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v4

      - name: Run Tests
        run: echo "Running tests..."

