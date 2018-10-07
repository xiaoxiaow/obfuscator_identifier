How to run
-----------------------------
1. copy the directory of apks into this folder. 
2. type "bash preprocess.sh name/of/the/apks/folder"
3. type "python classify.py | tee log"


Prerequest:
-----------------------------
1. Sklearing: http://scikit-learn.org/stable/install.html

There may be other required libraries. If you have any question, please
send me email.


To verify if the prerequest is met, I attached a test folder calld "test_apk".
So run it:
1. bash preprocess.sh test_apk
2. python classify.py | tee log

Then the result will be shown in both the screen and in the file called "log"
under this directory. 

Note:
----------------------------

The preprocess part may be time consuming if the number of apks is large.
There are five kinds of label:
1. Original ( not obfuscated by any of the four ones. We assume it has no obfuscation. But in fact, it may be obfuscated by other obfuscator) 
2. Proguard
3. Allatori
4. Legu
5. Bangcle

