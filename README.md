# Installation
To Install the .vsix package in Visual Studio Code:
1. Download the .vsix file from [here](https://we.tl/t-SRxrj82Kkj)
2. Open Visual Studio Code.
3. Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or by pressing Ctrl+Shift+X.
4. Click on the three dots in the top right corner of the Extensions view.
5. Select Install from VSIX…
6. Browse to the downloaded .vsix file generated and select it.

# Example Use Cases

The extension comes with several built-in commands to manage and interact with `dfx.json` and related development tasks. These commands are executed through the context menu in the Canisters View.

**Refresh**: When you have made changes to the `dfx.json` file outside of VS Code or through other processes and want to ensure the tree view is up-to-date.

`canisters> Show Actions`:

1. **Start the Replica**:
    
    - **Use Case**: When you need to start the local Internet Computer (IC) replica to test your canisters.
    - **Action**: Select “Start Replica” from the options menu to initiate the local IC instance.
2. **Deploy All Canisters**:
    
    - **Use Case**: When you want to deploy all canisters defined in the `dfx.json` file.
    - **Action**: Select “Deploy Canisters” from the options menu to deploy all canisters at once.
3. **Deploy Candid**:
    
    - **Use Case**: When you want to use Candid UI to test deployed canister methods in webview in VS Code.
    - **Action**: Select “Deploy Candid” from the options menu to deploy Candid UI canister.

`Show Canister Actions`:

1. **Deploy a Canister**:
    
    - **Use Case**: When you have made changes to a specific canister and need to deploy it.
    - **Action**: Click on the canister in the tree view and select “Deploy Canister”
2. **View Logs**:
    
    - **Use Case**: View logs for specific canister.
    - **Action**: Click on a canister and select “View Logs”
3. **Open Candid UI**:
    
    - **Use Case**: Open Candid UI in webview.
    - **Action**: Click on a canister which has been deployed and select “Open Candid UI”
4. **Open Candid UI in sidebar**:
    
    - **Use Case**: Open Candid UI in webview in sidebar.
    - **Action**: Click on a canister which has been deployed and select “Open Candid UI in sidebar”

`Deployed canisters`:

This is a menu view which shows deployed canisters and by selecting one of it you can open Candid UI with selected deployed canister in sidebar.

## Candid UI

For running Candid UI in this extension we changed authentication functionality by removing authentitcating user in Internet Identity canister and instead we added set of 10 random identities in Candid UI which are ready to use. They are generated from the same seed phrase `during nut robust trouble drip question series endless hurry upper track cost time bone crunch gorilla cause peasant fantasy prison banana toy toward mean` and with changed derivation path for next ones. Also we added functions to expand this set which are

- **Add new identity** - adds new random identity from the seed phrase pasted above
- **New identity from seed phrase** - adds new identity from the seed phrase given by user
- **New identity from private key** - adds new identity from private key given by user
