# sensibility_testbed

--Update 1/29--
yu_test_v3.r2py: replace reqeust with get_accelerometer, delete log in while loop
Hold_in_hand.m: add crossing zero method(with trick, only determine the signal above std(figuredMagNoG)), using butterworth filter to replace pre-emphasis filter(tried moving average, Binomial)


All *_matlab.csv is raw data from accelerometer, please paste the file name into the .m file to execute. All results and output figures are saved in each folder. The *_result.csv includes raw data and recorded steps data, and also saved the carrying method(hold in hand or keep in trousers pocket)

Pocket_step.m works for carrying the phone in the trousers pocket.
For example, the recorded steps is 321, and the estimated steps is 308
![alt tag](https://github.com/yh570/sensibility_testbed/blob/master/1_25_20_38_result/figure7.png)

Hold_in_hand.m works for carring the phone in coat pocket or hold in the hand.

yu_test_v3.r2py works to collect and record the data from accelerometer. The data will be stored in accelerometer_data

yu_test2.r2py works to collect and record the data from BOTH accelerometer and location together with a same clock. The data will be stored in accelerometr_data and location_data.

