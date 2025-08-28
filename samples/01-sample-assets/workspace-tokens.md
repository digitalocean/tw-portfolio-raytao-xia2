---
description: >-
  The AI Hub features Workspace tokens for accessing the AI Hub API. You can
  create Workspace tokens in the AI Hub as soon as you create an account.
---

# Workspace Tokens

{% hint style="danger" %}
Do not share Workspace tokens.
{% endhint %}

To access the AI Hub with PySDK, you'll need to create a Workspace token with the AI Hub. You can create Workspace tokens only if your account is part of a Workspace.

If you plan to use PySDK fully offline, or you plan to use models available in public Model Zoos, you don't need to create Workspace tokens.

Workspace tokens allow you to:

* Run cloud inference on models in public Model Zoos.
* Access to models in the Workspace Model Zoos for local and AI server inference.
* Run cloud inference on models in Workspace Model Zoos.

## Creating and managing tokens

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2FN2qU8yQ7u9vVPK6WYa1W%2Fimage.png?alt=media&#x26;token=63b4d30e-0961-4a25-b28f-1207985e720f" alt="AI Hub Tokens interface."><figcaption><p>AI Hub Tokens interface.</p></figcaption></figure>

To create or manage tokens, navigate to [Workspace tokens](https://hub.degirum.com/private-tokens) in the AI Hub. You'll be able to:

* Generate new tokens: Click the **Generate Workspace Token** button, then set a description and expiration date for the token.
* View partial token keys: The Tokens interface will display part of the token key for existing tokens. You will not be able to view the entire token key through the interface.
* Copy token keys: Click the copy action button to the right of the token key to copy the token key.
* Delete tokens: Click the delete action button to the right of the token key to delete the key. A confirmation popup will appear to confirm if you want to delete the key.

If you have PySDK installed, you may also use a PySDK CLI helper to manage tokens easily over a terminal. [Click here](../../../pysdk/user-guide-pysdk/command-line-interface#manage-ai-hub-tokens) for more information about the PySDK CLI helper.
