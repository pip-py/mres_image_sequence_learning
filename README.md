# SimVPv2 for Image Sequence Interpolation and Extrapolation 2025-01



<p align="center">
  <img src="https://github.com/user-attachments/assets/0042474e-6a42-40a1-874e-bcf43b2f5053" alt="Image Sequence Example"/>
</p>

From paper:

### Data Example of autoregressive process

<p align="center">
  <img src="https://github.com/user-attachments/assets/cfbf1854-e240-4782-8ee1-db92b6872aa2" alt="Image Sequence Example"/>
</p>

### Example of Model Output on Test:

<p align="center">
  <img src="https://github.com/user-attachments/assets/2040b3fc-992b-4975-b753-f9c5418b4b8f" alt="Model Output Example"/>
</p>


### Full Assignment Doc:

[**Link to PDF**](https://github.com/pip-py/mres_image_sequence_learning/blob/main/JM_AMML_Assignment_2025_v3.pdf)


### My reflection:
Personal circumstances made the completion of the two Autumn term summative assignments and exam difficult and not as much time as I had hoped were spent completing, validating and checking. 

I began this process looking into building an auto-encoder where the latent variables would feed directly into a transformation matrix which would augment the original image as a decoder. e.g. laten var 1 -> rotation theta -> latent var 2 dx ... etc. However, the design of this failed to train effectively and was due to the connection of the loss function when performing the backward pass. I returned to SimVPV2 and with some fiddling, able to get OpenSTL up and running on A100 on colab. I consistenly underestimate training time as in my formative and for my dissertation I will move away from solely jupyter and colab as trialled in my autumn summatives and perform my experiments in a different environment which will prevent time-out and promote parallelism more. 

Despite the flaws of my work, I effectively implemented SimVPv2 on a novel problem with the magic of interpolation and extrapolation coming from transformation of the training data. 


<p align="center">
  <img src="https://github.com/user-attachments/assets/bdc529cb-1a0b-4635-aa5f-ea955526ad8d" alt="Model Output Example"/>
</p>
