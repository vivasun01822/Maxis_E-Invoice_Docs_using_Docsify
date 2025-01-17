# Json Transformer

The Json Transformer section provides an easy way to transform JSON documents into `UBL 2.1` documents. After the transformation, you can submit the transformed documents to IRBM and then receive the submission response from IRBM server.


![Json Transformer Overview](../_media/jsonTransformer1.png)


The Json Transformer is divided into two parts. They are:


### Input Json 

In the Input JSON section, you can enter one or more JSON documents. The total number of documents must not exceed `100`, and the file size should remain under `5 MB`. Two buttons are provided: one to clear the input field and another to transform the documents. You can also download a sample JSON file by clicking the down arrow button. After transforming the documents, you will see a toast message that `Successfully Transform`. 

![Input Json](../_media/jsonTransformer2.png)


### Submit Transformed Documents

In order to submit transformed documents to IRBM, you must provide the `Data Source` of those documents. Then you can submit it to the IRBM. You can also download transformed documents by clicking the down arrow button. 

![Transformer Json](../_media/jsonTransformer3.png)

By clicking the `Submit to IRB button`, you will see a success or error message on top of the input field.

![Submit Transformed Json](../_media/jsonTransformer4.png)