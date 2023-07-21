# My first try at github actions

## Deploy a simple infra piece through github actions

## Set up
### Configuring github actions and connecting it to AWS

1. Create a file in ./github/workflows
2. Set up an IAM user for github to assume and generate access keys
3. Add the credentials to github secrets
4. Just create your stack! 

### Improvement: Using roles instead of users
Using a user is discouraged, since it requires that AWS persistent crediential are stored in the repo. Instead we can use roles and let github actions assume the role when needed. To set up the role follow the instructions here https://aws.amazon.com/blogs/security/use-iam-roles-to-connect-github-actions-to-actions-in-aws/


