# i-learn-gee-sea-pea
Playing with GCP for the "GCP Fundamentals for AWS Pro's" course on Coursera

## Useful commands
- Generate service account cred's: `gcloud iam service-accounts keys create ./key.json --iam-account=<sa_name>@<project_id>.iam.gserviceaccount.com`
- Set SA cred's for TF: `export GOOGLE_APPLICATION_CREDENTIALS="./key.json"`
- SSH into compute instance: `gcloud beta compute ssh --zone "us-east1-b" "<instance_id>"  --tunnel-through-iap --project "<project_id>"`