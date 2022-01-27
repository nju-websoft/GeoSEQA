# GeoSEQA

Scenario-based question answering (SEQA) is to answer a question which is contextualized by a scenario and expects a paragraph-long answer. A scenario may contain text and images to describe a concrete case in the domain. GeoSEQA is a SEQA dataset containing 4,003 scenario-based essay questions collected from China's high-school geography exams. We  randomly  split  the  4,003  questions  into 2,393  for  training  (59.8%),  781  for  validation(19.5%),  and  829  for  test  (20.7%). 

## dataset

The train_raw.json, val_raw.json and test_raw.json files consist question, answer and scenario( material, image and image_text):

```python
{
    "id":"id",
    "background_id":"background_id",
    "src":"question",
    "tgt":"gold-standard answer",
    "material":["text scenario",...],
    "image":[["image title","image annotation by template"],...],
    "image_text":[["image title","image annotation by natural language"],...],
    "object2Geonames":{"value of entity slot in image annotation by template":{"longitude"：longitude,"latitude"：latitude},...}
}
```



