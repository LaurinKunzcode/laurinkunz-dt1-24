# laurinkunz-dt1-24

# Introduction
This project involves deploying a Flask-based application as a proxy for the Hugging Face Inference API, hosted on a Google Cloud Platform (GCP) virtual machine (VM). The application is containerized using Docker, with a frontend integration planned via Retool. The purpose of this project is to demonstrate concepts in software architecture, API design, and cloud computing.

## Account Details
DockerHub: laurinkunz
Hugging Face: Laurincode
GitHub: laurinKunzcode
Retool Link: <[https://bfhdt1.retool.com/apps/b4d5727c-a270-11ef-955d-8bf96eb9e217/Assignment_DT1-24](https://laurinkunz.retool.com/apps/6927ab90-a326-11ef-bbc3-937c8620121b/Untitled)


# VM instances_Google Cloud
VM instances_External IP: 34.45.52.25

## Firewall

Disallow IP:
0.0.0.0/0

Allow Retool IPs:
// 3.77.79.248/30
// 3.77.79.248
// 3.77.79.249
// 3.77.79.250
// 3.77.79.251
// 35.90.103.132/30
// 44.208.168.68/30
// 35.90.103.132
// 35.90.103.133
// 35.90.103.134
// 35.90.103.135
// 44.208.168.68
// 44.208.168.69
// 44.208.168.70
// 44.208.168.71

Allow CIDR Address: 
147.87.0.0/16


# System Architecture
## Components:
GCP Virtual Machine: Hosts the backend application.
Docker Container: Encapsulates the Flask app and dependencies.
Hugging Face API: Provides text generation capabilities.
Retool: A no-/low-code platform for the frontend interface.

## Data Flow:
User inputs are sent from Retool to the Flask application.
The Flask app communicates with the Hugging Face API and returns results.
Responses are displayed on the Retool interface.
