# Cloud run deployment demo

Usees [direct WIF](https://github.com/google-github-actions/auth#direct-wif) 
See also: https://github.com/docker/login-action?tab=readme-ov-file#google-artifact-registry-gar

##  Wanted roles for deploying to cloud run
# https://cloud.google.com/blog/products/devops-sre/deploy-to-cloud-run-with-github-actions/
- [x] roles/artifactregistry.writer
- [ ] roles/iam.serviceAccountUser
- [x] roles/run.admin
- [ ] roles/iam.workloadIdentityUser


### Continuous integration step
- Check out the repository
- Build container image (docker)
- ... some auth step here to be allowed to push
- Push container image to artifact registry

### Continuous deployment step


Relevant actions:
- [deploy-cloudrun](https://github.com/google-github-actions/deploy-cloudrun)

## Some links
- Cloud run URL: https://cloud-run-deploy-747268936816.europe-west1.run.app/
- Artifact registry https://console.cloud.google.com/artifacts/docker/ancient-sunspot-352209/europe-west1/cloud-run-deploy-repo/cloud-run-deploy?inv=1&invt=Abh1_A&project=ancient-sunspot-352209
