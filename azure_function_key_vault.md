# Integrate Azure Functions with Azure Key Vault

By default Azure Functions store it Key in a blob storage container where they are not easy to access.

A better alternative is to configure the Azure Function to store all keys into a Key Vault where a different application can access the key safely.

The approach how to do it is well described in the the following blog entry:
[How to store function app's function keys in a key vault](https://techcommunity.microsoft.com/t5/apps-on-azure-blog/how-to-store-function-app-s-function-keys-in-a-key-vault/ba-p/2639181)

There was a change on how to configure the reference to the Azure Key Vault. This is described in the following Github Issue:
[Update the Key Vault secret provider to use Azure.Identity](https://github.com/Azure/Azure-Functions/issues/2048)