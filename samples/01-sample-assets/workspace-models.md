---
description: >-
  Read this page to learn about how to navigate and create model zoos in the
  DeGirum AI Hub. All users have access to the model zoo. The ability to create
  model zoos is on a per-workspace basis.
---

# Workspace Models

If your Workspace has permission, you can create Workspace Model Zoos for your Workspace.

## Creating a Workspace Model Zoo

If your Workspace has permission to create Model Zoos:

{% stepper %}
{% step %}
**Click Models in the navigation bar on the left**

You will see tiles for Model Zoos and All Models. Click the Model Zoos tile.

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2FMJHlsff4vgSoctopU4lQ%2Fimage.png?alt=media&#x26;token=2334bb6a-72e8-49a9-b5ba-382e866033d1" alt=""><figcaption><p>Model Zoos and All Models Tiles</p></figcaption></figure>
{% endstep %}

{% step %}
**Click New Model Zoo**

After you click the Model Zoos tile, you will be brought to the list of model zoos.

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2Fgit-blob-6819fb1725893899592d3f40753fa6d4d8b00199%2Fimage.png?alt=media" alt="" width="563"><figcaption><p>New Model Zoo button when viewing Model Zoos</p></figcaption></figure>

If enabled for your Workspace, there will be a New Model Zoo button. Click the New Model Zoo button.
{% endstep %}

{% step %}
**Set up the Model Zoo**

After you click the New Model Zoo button, a window opens with a menu to set up the model zoo.

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2Fgit-blob-40b5f87d223165e1dfe053b872020c46c2595331%2Fimage.png?alt=media" alt="" width="563"><figcaption><p>New Model Zoo form</p></figcaption></figure>

* Model Zoo Name: Name of the model zoo.
* Model Zoo Description: Description of the model zoo.
{% endstep %}

{% step %}
**Click Add New Model Zoo**

The Model Zoo will be created for your Workspace.
{% endstep %}
{% endstepper %}

## Viewing all models in your Workspace

You can easily view all models available in your Workspace.

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2FMJHlsff4vgSoctopU4lQ%2Fimage.png?alt=media&#x26;token=2334bb6a-72e8-49a9-b5ba-382e866033d1" alt=""><figcaption><p>Model Zoos and All Models Tiles</p></figcaption></figure>

To view all models:

{% stepper %}
{% step %}
**Click Workspace Models in the navigation bar on the left**

You will see tiles for Model Zoos and All Models.
{% endstep %}

{% step %}
**Click All Models**

After clicking the All Models tile, you will see a directory of models. You will also see a search/filter panel to search and filter models.
{% endstep %}
{% endstepper %}

To view all models in a Workspace:

{% stepper %}
{% step %}
**Select a Workspace in the navigation bar on the left**

The Workspace you have selected will determine what models you can view.
{% endstep %}

{% step %}
**Click Workspace Models**

You will see tiles for Model Zoos and All Models.
{% endstep %}

{% step %}
**Click All Models**

After clicking the All Models tile, you will see a directory of models. You will also see a search/filter panel to search and filter models. This directory of models features only models in the Workspace you selected; it will not feature any models available in the public Model Zoo. Likewise, the search/filter panel will filter only models in the Workspace.
{% endstep %}
{% endstepper %}

## Models Directory Page

The Models Directory page displays information about models and provides a few action buttons.

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2Fgit-blob-4cbf436a5a305ffb91f80981ec72a1ca564158a7%2Fimage.png?alt=media" alt=""><figcaption><p>Models Directory Page</p></figcaption></figure>

* Name: Identifies each model. We provide a recommended naming convention for models in our documentation about [organizing models](../../pysdk/user-guide-pysdk/organizing-models) for DeGirum PySDK.
  * If you are viewing all models, the Models Directory Page will also indicate the workspace and zoo where the model lives.
* Devices: Hardware compatibility of the model. This information is retrieved from the model JSON file.
* Version: Version number of each model. This information is retrieved from the model JSON file.
* Action Buttons:
  * Edit: Opens a window to edit the model readme, model JSON file, and labels JSON file. You will need the right permissions to use this action button.
  * Download: Downloads a zip file containing the model, model JSON file, and labels JSON file.
  * Copy: Copies the model to a different model zoo controlled by your workspace. You will need the right permissions to use this action button.
  * Delete: Deletes the model from the model zoo. You will need the right permissions to use this action button.

If you are viewing a specific model zoo, the models page features:

* Model Zoo Action Buttons: Buttons to copy the Model Zoo AI Hub path, edit the Model Zoo, and delete the Model Zoo. The edit and delete action buttons are identical to the edit and delete action buttons available in the [Model Zoos](#model-zoos-page) page. You will need the right permissions to use this action button.
* New Model button: Allows you to upload a new model if your workspace created the Model Zoo. To upload a model, you must prepare a zip file containing the model, model JSON, and labels JSON all in one archive. The max size of this zip file is 1 GB. The Models Directory page will automatically identify information about the model based on the contents of the JSON file in the uploaded archive.
* Pagination Controls: Navigates through pages of models.

### Search/Filter Panel When Viewing the Models Directory Page

When viewing the Models Directory page, the search/filter panel enables searching by model name and filtering by device type, quantization, and output postprocessor type.

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2FMUJlcH4hgpUPYW1dVLdP%2Fimage.png?alt=media&#x26;token=ba741279-4772-4dea-b2fa-47d5199640a7" alt="" width="563"><figcaption><p>Search/Filter Panel for the Models Directory Page</p></figcaption></figure>

Click Quick Search and enter text to search the model list for model names matching your search.

Click buttons for Device Type, Quantization, and Output Postprocessor Type to filter models.

* Device Type: Hardware compatibility of the model.
* Quantization: Whether the model is a floating point model or a quantized model. Quantized models typically perform much faster than floating point models.
* Output Postprocessor Type: The type of postprocessor file used by the model. Most models use postprocessors, but some models do not require postprocessors.

## Viewing Model Zoos

{% stepper %}
{% step %}
**Verify that you have your Workspace selected**

Your selected Workspace determines which model zoos you can view. Select your Workspace using the Workspace dropdown in the left navigation bar.
{% endstep %}

{% step %}
**Click Workspace Models in the Navigation Bar on the Left**

You will see tiles for Model Zoos and All Models. Click the Model Zoos tile.
{% endstep %}

{% step %}
**View Available Model Zoos**

After clicking the Model Zoos tile, you will see tiles for model zoos. You will also see a search/filter panel to search and filter model zoos.
{% endstep %}
{% endstepper %}

## Model Zoos Page

The Model Zoos page displays model zoo tiles and provides a few action buttons.

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2Fgit-blob-fabf5c86d4a540bc29ad260f7dde2bf4f7bf8379%2Fimage.png?alt=media" alt="" width="563"><figcaption><p>Model Zoos page</p></figcaption></figure>

Each model zoo tile follows this format:

* Model Zoo Name: Identifies each model zoo. Written in bold.
* Workspace: The workspace that created the model zoo. Written in italics beneath the model zoo name.
* Action Buttons:
  * Edit: Opens a window to edit the model zoo name and description. You will need the right permissions to use this action button.
  * Visibility: Displays the model zoo's visibility.
  * Delete: Deletes the model zoo. Opens a confirmation pop-up to confirm deletion of the selected model zoo. Deleted model zoos cannot be restored.

Additionally, the Model Zoos page features:

* Sort Controls: Sort the model zoo tiles by model count or alphabetically in descending order.
* Pagination Controls: Navigates through pages of model zoo tiles.

### Search/Filter Panel When Viewing Model Zoos

When viewing model zoos, the search/filter panel enables searching by model zoo name and filtering by organization and visibility.

<figure><img src="https://951436927-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKrw9MoaNbGYR2wt03kN0%2Fuploads%2FSyhbhk9MxmdgSQFxUaWv%2Fimage.png?alt=media&#x26;token=cc1ea50a-ed12-43e0-9012-566436b24a2a" alt=""><figcaption><p>Search/Filter Panel for the Model Zoos page</p></figcaption></figure>

Click Quick Search and enter text to search the model zoos for model zoos matching your search.

Click buttons for organization and visibility to filter models.

* Organization: The workspace that created the model zoo.
* Visibility: Indicates whether the model zoo is **Private**, **Shared Private**, or **Public**. All zoos created by workspaces are private. Only DeGirum publishes public model zoos.
