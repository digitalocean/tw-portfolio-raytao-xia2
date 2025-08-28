---
description: >-
  Port and optimize your custom AI models for various hardware platforms using
  DeGirum’s Cloud Compiler.
---

# Cloud Compiler

The DeGirum Cloud Compiler simplifies the process of preparing AI models for real-world deployment. It takes PyTorch checkpoints—specifically models trained using the Ultralytics repository—and compiles them into formats that run efficiently on supported edge AI hardware.

Upload your PyTorch checkpoint to the Cloud Compiler and let it handle the conversion. You can adjust parameters to optimize performance, choose target runtimes and devices, and provide a custom dataset for quantization to meet your deployment requirements.

When a model is compiled, it can be loaded [online or offline with PySDK](../../pysdk/quickstart) or run directly in the browser with the [Model Console](../model-console).&#x20;

The Cloud Compiler currently supports models for these runtimes, devices, and precisions:

| Runtime  | Devices                | Precision support |
| -------- | ---------------------- | ----------------- |
| HAILORT  | HAILO8, HAILO8L        | Quant only        |
| DEEPX    | M1A                    | Quant only        |
| AXELERA  | METIS                  | Quant only        |
| OPENVINO | CPU, NPU, GPU          | Float and quant   |
| MEMRYX   | MX3                    | Float only        |
| TFLITE   | CPU, EDGETPU           | Float and quant   |
| N2X      | CPU, ORCA1             | Float and quant   |
| RKNN     | RK3566, RK3568, RK3588 | Float and quant   |

### Using the Cloud Compiler

Access to the Cloud Compiler is on a per-workspace basis.

When your workspace has access to the Cloud Compiler, you will be able to access the Cloud Compiler. Without access, you can request early access for your workspace to the Cloud Compiler through the form available in the Cloud Compiler section of the AI Hub.

{% stepper %}
{% step %}
**Select a Workspace with Cloud Compiler access**

Click the Workspace dropdown menu in the left-hand navigation bar of the AI Hub, and select a Workspace with Cloud Compiler access.
{% endstep %}

{% step %}
**Create or get access to a Model Zoo**

The Cloud Compiler places compiled models into a model zoo. Ensure you have a model zoo where you can upload pre-compiled models.

To learn how to create Model Zoos, [click here](../workspace-models#creating-a-model-zoo).
{% endstep %}

{% step %}
**Visit the Cloud Compiler page**

After ensuring you have access to a Model Zoo where you can upload models, click Cloud Compiler in the AI Hub navigation bar to visit the Cloud Compiler page.
{% endstep %}

{% step %}
**Upload a checkpoint file**

Click **Upload File** to submit a PyTorch checkpoint (.pt) for compilation.
{% endstep %}

{% step %}
**Fill out the Details section**

In the Details section, fill in details such as name prefix, version, image width, and image height to identify your model in the model zoo.
{% endstep %}

{% step %}
**Select a Model Zoo in the Details section**

Choose the Model Zoo where the compiled model will be published.

If the Model Zoo selector is empty, then recheck if you have created or can access a Model Zoo where you can upload pre-compiled mode.
{% endstep %}

{% step %}
**Select a runtime and device in the Target section**

In the Target section, choose the target runtime, device, and type from the dropdown menus. The Cloud Compiler uses your selections to build your model.
{% endstep %}

{% step %}
**Select advanced options (optional)**

Each runtime and device offers advanced options. View the advanced options to further optimize your model, such as by uploading a calibration dataset for quantization.
{% endstep %}

{% step %}
**Start model compilation**

Click **Compile** to start. The Cloud Compiler task will appear in the task list available when you click Tasks in the AI Hub navigation bar. When the process completes, your model is published to the selected model zoo, and you will receive an email confirming that the model has been compiled.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Some runtime, device, and type combinations support multiple devices. The device you select in the form will be the device in the resulting model .json's `DeviceType` field, while all supported devices using the same runtime will be listed in the `SupportedDeviceTypes` field.

[Click here](../../pysdk/user-guide-pysdk/model-json-structure) for more information about the model .json file.
{% endhint %}
