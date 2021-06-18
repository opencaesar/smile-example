# SMILE Example

[![Build Status](https://travis-ci.com/opencaesar/smile-example.svg?branch=master)](https://travis-ci.com/opencaesar/smile-example)
[![Release](https://img.shields.io/github/v/tag/opencaesar/smile-example?label=release)](https://github.com/opencaesar/smile-example/releases/latest)
[![Documentation](https://img.shields.io/badge/Documentation-HTML-orange)](https://opencaesar.github.io/smile-example/) 
[![Gitpod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/opencaesar/smile-example) 

This is a description of a "Space Multi-mission Infrastructure for Lunar Exploration" (SMILE) project expressed in [OML](https://github.com/opencaesar/oml)

Note: check above buttons setup

## Clone
```
  git clone https://github.com/opencaesar/smile-example.git
  cd smile-example
```

## Build
Equivalent to owlReason task
```
./gradlew build
```

## Generate Docs
You must first have Bikeshed (the app itself) installed from [here](https://tabatkins.github.io/bikeshed/#install-final)
```
./gradlew generateDocs
```

## Run OWL Reasoner
```
./gradlew owlReason
```

## Start Fuseki Server
```
./gradlew startFuseki
```

## Stop Fuseki Server
```
./gradlew stopFuseki
```

## Load to Fuseki Dataset
```
./gradlew owlLoad
```
Pre-req: A Fuseki server with a firesat dataset must be running at http://localhost:3030/firesat (see below)  

## Run SPARQL Queries
```
./gradlew owlQuery
```
Pre-req: A Fuseki server with a firesat dataset must be running at http://localhost:3030/firesat (see below)  

## Run SHACL Rules
```
./gradlew owlShacl
```
Pre-req: A Fuseki server with a firesat dataset must be running at http://localhost:3030/firesat (see below) 

## Publish to Maven Local
```
./gradlew publishToMavenLocal
```
