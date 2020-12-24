# BBD:Bimodel Backdoor Defence

BBD is a Backdoor Defence Technique design for correctly recognize clean data and identify poisoned data as `N+1` Label.

## Group Member

Yunrui Huang(yh2910)

Yihong Wang(yw3408)

Jiru Wang(jw6288)

Yichen Wang(yw4604)

## Evironment

`Python=>3.x`

`Jupyter Notebook`

`Tensorflow == 1.x`(for`neural_clease.ipythnb` to run)

`tensorflow-model-optimization`

`Keras => 2.x`

`h5py`

## Run Instruction 

 To run source code in `/src`, please files in Jupyter Notebook and modify data and model path into customized path.

`Fine_Pruning_Weight_Pruning.ipynb`

* `clean_data_filename` => customized clean validation data path
* `test_data_filename` =>customized clean test data path
* `poison_data_filename`=>customized poison data path

`Fine_Pruning_activation_based.ipynb`

* `clean_data_filename` => customized clean validation data path
* `test_data_filename` =>customized clean test data path
* `poison_data_filename`=>customized poison data path

`Entropy_filter.ipythnb`

* `clean_data_filename` =>customized clean validation data path

* `test_clean_data_filename` =>customized clean test  data path

* `poison_data_filename` => customized poison data path

  

`neural_clease.ipythnb`

* `DATA_DIR` => customized data folder

* `DATA_FILE` => customized clean data path

* `MODEL_DIR` => customized model folder

* `MODEL_FILE` => customized Badnet path

  

`BBD.ipythnb`

* `DATA_DIR` => customized data folder
* `CLEAN_DATA_FILE` => customized clean validation data path
* `POISON_DATA_FILE`=> customized poison data path
* `MODEL_DIR` => customized model folder
* `BAD_MODEL_FILE` => customized Badnet path
* `CLEAN_MODEL_FILE` => customized clean model path

All files can run idenpendently and with differnt purpose.



## File Describtion

| File                                | Input                      | Output              | Describtion |
| ----------------------------------- | -------------------------- | ------------------- | ----------- |
| `neural_clease.ipythnb`             | `<Badnet, Clean_Data>`     | `potential_trigger` |             |
| `Fine_Pruning_Weight_Pruning.ipynb` | `<Badnet, Clean_Data>`     | `Repaired_Model`    |             |
| `Fine_Pruning_activation_based.ipynb` | `<Badnet, Clean_Data>`     | `Repaired_Model`    |             |
| `Entropy_filter.ipythnb`            | `Badnet`                   |                     |             |
| `BBD.ipythnb`                       | `<Badnet, Repaired Model>` |                     |             |

