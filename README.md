# OpenFn Docker Setup

## Introduction

This repo contains a production setup of the openFn tool'

## Prerequisites

You need to have latest docker installed

## Setting up

Clone this repository

```bash
git clone https://github.com/hisptz/openfn-docker
```

Then, create an env file, copy the existing file for simplicity

```bash
cp .env.example .env
```

Then change all the variables in the `.env` file. Make sure the keys are generated well. Ensure the `SECRET_KEY` is more
than 64 characters long

## Running

To run the app run

```bash
 docker compose up -d 
```

Your app should be available at the port you configured in the `.env` file (http://localhost:4000 if you use the default
port).

## Upgrading

To upgrade any of the images simply run 
```bash 
docker compose up -d --pull always
```
Ensure you read the release notes to abide to any other changes you have to do.

