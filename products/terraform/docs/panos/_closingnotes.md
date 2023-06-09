## Closing notes

- Note that when working with Terraform at scale and in production, the code would likely be split into several `.tf` files for the provider section, the variable section, and the rest of the code. For the purposes of this learning tutorial, keeping the code in a single file works fine.
- The PAN-OS credentials are being stored within the code and on disk unencrypted. This is not a production-level solution, and other solutions for managing secrets should be considered for real-world deployments. Hashicorp (owners of Terraform) and many others have solutions for this.
- Almost all values were defined within the code; names of configuration items, IP addresses, and more. This is very suitable for a learning tutorial, but this approach does not scale well in production, and using variables instead is something to consider as you operationalize Terraform within your organization.
