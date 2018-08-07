README

This file contains all data used on paper "Analyzing and Increasing the Reliability of
Convolutional Neural Networks on GPUs"


Please do not distribute data until the paper is published.

Data is organized in the following files:


-- sassifi_inst: contains all errors obtained on fault injections using INST mode

-- sassifi_rf: contains all errors obtained on fault injections using RF mode


-- ecc_on: contains all observed errors under the beam for K40 with ECC enabled

-- ecc_off: contains all observed errors under the beam for K40 (ECC OFF), Titan X, and X




Each file is organized as follows:



BENCHMARK_AND_MACHINE_NAME: which could be cudaDarknet_carol-k402 for YOLO(Darknet) on K40, PyFasterRcnn_carol-k402 Faster RCNN on K40, cudaDarknet_carolx1 Darknet on Tegra X1, PyFasterRcnn_carol-tx Faster RCNN on Titan X or cudaDarknet_carol-tx Darknet on Titan X
log_name:\

Each log output file which contains:
-date and time of the test
sdc_iteration
-iteration of SDC, once not all executions produced SDC
-
it_errors: how many errors in this SDC
-
ERROR_LIST
All errors listed, to compare with golden value the errors are printed always using the value read (x_r, y_r, prob_r for object probability, h_r for height, w_r for width) and expected value (x_e, y_e, prob_e for object probability, h_e for height, w_e for width)
