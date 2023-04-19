# Comparing `tmp/PeakDetective-0.1.4.tar.gz` & `tmp/PeakDetective-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PeakDetective-0.1.4.tar", last modified: Mon Jan 30 18:47:55 2023, max compression
+gzip compressed data, was "dist\PeakDetective-0.1.6.tar", last modified: Wed Apr 19 20:20:05 2023, max compression
```

## Comparing `PeakDetective-0.1.4.tar` & `PeakDetective-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-30 18:47:55.000000 PeakDetective-0.1.4/
--rw-rw-rw-   0        0        0      712 2023-01-30 18:47:55.000000 PeakDetective-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-30 18:47:55.000000 PeakDetective-0.1.4/PeakDetective/
--rw-rw-rw-   0        0        0    40889 2023-01-30 16:18:16.000000 PeakDetective-0.1.4/PeakDetective/__init__.py
--rw-rw-rw-   0        0        0     9999 2023-01-30 18:17:39.000000 PeakDetective-0.1.4/PeakDetective/detection_helper.py
--rw-rw-rw-   0        0        0     1715 2023-01-30 16:28:13.000000 PeakDetective-0.1.4/PeakDetective/find_peaks.R
--rw-rw-rw-   0        0        0      340 2023-01-29 14:48:51.000000 PeakDetective-0.1.4/PeakDetective/install_R_packages.R
--rw-rw-rw-   0        0        0     1978 2023-01-19 22:58:22.000000 PeakDetective-0.1.4/PeakDetective/mz_unity.R
-drwxrwxrwx   0        0        0        0 2023-01-30 18:47:55.000000 PeakDetective-0.1.4/PeakDetective.egg-info/
--rw-rw-rw-   0        0        0      712 2023-01-30 18:47:54.000000 PeakDetective-0.1.4/PeakDetective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-01-30 18:47:54.000000 PeakDetective-0.1.4/PeakDetective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-30 18:47:54.000000 PeakDetective-0.1.4/PeakDetective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-01-30 18:47:54.000000 PeakDetective-0.1.4/PeakDetective.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-30 18:47:54.000000 PeakDetective-0.1.4/PeakDetective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-30 18:47:55.000000 PeakDetective-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-01-30 18:46:45.000000 PeakDetective-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/
+-rw-rw-rw-   0        0        0      712 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective/
+-rw-rw-rw-   0        0        0    45471 2023-04-06 17:44:24.000000 PeakDetective-0.1.6/PeakDetective/__init__.py
+-rw-rw-rw-   0        0        0    11229 2023-03-21 22:15:29.000000 PeakDetective-0.1.6/PeakDetective/detection_helper.py
+-rw-rw-rw-   0        0        0     1715 2023-01-30 16:28:13.000000 PeakDetective-0.1.6/PeakDetective/find_peaks.R
+-rw-rw-rw-   0        0        0      340 2023-01-29 14:48:51.000000 PeakDetective-0.1.6/PeakDetective/install_R_packages.R
+-rw-rw-rw-   0        0        0     1978 2023-01-19 22:58:22.000000 PeakDetective-0.1.6/PeakDetective/mz_unity.R
+drwxrwxrwx   0        0        0        0 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/
+-rw-rw-rw-   0        0        0      712 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/PeakDetective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:20:05.000000 PeakDetective-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-04-19 20:14:53.000000 PeakDetective-0.1.6/setup.py
```

### Comparing `PeakDetective-0.1.4/PKG-INFO` & `PeakDetective-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: PeakDetective
-Version: 0.1.4
+Version: 0.1.6
 Summary: Curates and detects LC/MS peaks in metabolomics datasets
 Home-page: https://github.com/e-stan/PeakDetective/
 Author: Ethan Stancliffe
 Author-email: estancl1234@gmail.com
 License: MIT
-Download-URL: https://github.com/e-stan/PeakDetective/archive/v0.1.4.tar.gz
+Download-URL: https://github.com/e-stan/PeakDetective/archive/v0.1.6.tar.gz
 Description: UNKNOWN
 Keywords: Metabolomics,LC/MS,Deep Learning,semi-supervised learning,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PeakDetective-0.1.4/PeakDetective/__init__.py` & `PeakDetective-0.1.6/PeakDetective/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,256 +18,143 @@
 from fastdtw import fastdtw
 from scipy.interpolate import interp1d
 import pickle as pkl
 import os
 import sklearn.metrics as met
 import datetime
 
-#Utility functions:
-def startConcurrentTask(task,args,numCores,message,total,chunksize="none",verbose=True):
-
-    if verbose:
-        m = Manager()
-        q = m.Queue()
-        args = [a + [q] for a in args]
-        t = Thread(target=updateProgress, args=(q, total, message))
-        t.start()
-    if numCores > 1:
-        p = Pool(numCores)
-        if chunksize == "none":
-            res = p.starmap(task, args)
-        else:
-            res = p.starmap(task, args, chunksize=chunksize)
-        p.close()
-        p.join()
-    else:
-        res = [task(*a) for a in args]
-    if verbose: t.join()
-    return res
-
-def safeNormalize(x):
-    """
-    Safely normalize a vector, x, to sum to 1.0. If x is the zero vector return the normalized unity vector
-    """
-    if np.sum(x) < 1e-6:
-        tmp = np.ones(x.shape)
-        return tmp / np.sum(tmp)
-    else:
-        return x/np.sum(x)
-
-def normalizeMatrix(X):
-    """
-    Normalize a matrix so that the rows of X sum to one
-    """
-    return np.array([safeNormalize(x) for x in X])
-
-def classify(preds):
-    """
-    Classify predictions, preds, by returning the index of the highest scoring class
-    """
-    classes = np.zeros(preds.shape)
-    for x in range(len(preds)):
-        classes[x,list(preds[x]).index(np.max(list(preds[x])))] = 1
-    return classes
-
-
-def take_closest(myList, myNumber):
-    """
-    Assumes myList is sorted. Returns closest value to myNumber.
-
-    If two numbers are equally close, return the smallest number.
-    """
-    pos = bisect_left(myList, myNumber)
-    if pos == 0:
-        return myList[0]
-    if pos == len(myList):
-        return myList[-1]
-    before = myList[pos - 1]
-    after = myList[pos]
-    if after - myNumber < myNumber - before:
-        return after
-    else:
-        return before
-
-
-
-def printProgressBar(iteration, total, prefix='', suffix='', decimals=1, length=50, fill='█', printEnd="\r"):
-    """
-    Call in a loop to create terminal progress bar
-    @params:
-        iteration   - Required  : current iteration (Int)
-        total       - Required  : total iterations (Int)
-        prefix      - Optional  : prefix string (Str)
-        suffix      - Optional  : suffix string (Str)
-        decimals    - Optional  : positive number of decimals in percent complete (Int)
-        length      - Optional  : character length of bar (Int)
-        fill        - Optional  : bar fill character (Str)
-        printEnd    - Optional  : end character (e.g. "\r", "\r\n") (Str)
-    """
-    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
-    filledLength = int(length * iteration // total)
-    bar = fill * filledLength + '-' * (length - filledLength)
-    print(f'\r{prefix} |{bar}| {percent}% {suffix}', end=printEnd)
-    # Print New Line on Complete
-    if iteration == total:
-        print()
-
-def updateProgress(q, total,message = ""):
-    """
-    update progress bar
-    """
-    counter = 0
-    while counter != total:
-        if not q.empty():
-            q.get()
-            counter += 1
-            #if counter % 20 == 0:
-            printProgressBar(counter, total,prefix = message, printEnd="")
-
-
-def getIndexOfClosestValue(l,v):
-    """
-    get index of list with closest value to v, assumes l is sorted
-    """
-    pos = bisect_left(l, v)
-    if pos == 0:
-        return 0
-    if pos == len(l):
-        return pos - 1
-    before = l[pos - 1]
-    after = l[pos]
-    if after - v < v - before:
-        return pos
-    else:
-        return pos - 1
-
 
 class PeakDetective():
     """
     Class for curation/detection of LC/MS peaks in untargeted metabolomics data
     """
-    def __init__(self,resolution=100,numCores=1,windowSize = 1.0):
+    def __init__(self,resolution=60,numCores=1,windowSize = 1.0):
+        """
+        Constructor for PeakDetective object
+        @param resolution: int, number of datapoints to sample in the EIC window
+        @param numCores: int, number of processor cores to use for concurrent computations
+        @param windowSize: float, size of EIC window to extract (in minutes)
+        """
         self.resolution = resolution
         self.numCores = numCores
         self.windowSize = windowSize
         self.smoother = Smoother(resolution)
         self.classifier = ClassifierLatent(5)
         self.encoder = keras.Model(self.smoother.input, self.smoother.layers[7].output)
 
     def save(self,path):
+        """
+        Save model weights to given path
+        @param path: str, path where weights should be saved
+        @return: None
+        """
         if not os.path.exists(path): os.mkdir(path)
         pkl.dump([self.resolution,self.windowSize],open(path+"parameters.pd","wb"))
         self.smoother.save(path + "smoother.h5")
         self.classifier.save(path+"classifier.h5")
         self.encoder.save(path+"encoder.h5")
 
 
     def load(self,path):
+        """
+        Load model weights
+        @param path: str, path to folder where model weights were saved
+        @return: None
+        """
         try:
             [self.resouton,self.windowSize] = pkl.load(open(path + "parameters.pd","rb"))
             self.smoother = keras.models.load_model(path+"smoother.h5")
             self.classifier = keras.models.load_model(path+"classifier.h5")
             self.encoder = keras.models.load_model(path+"encoder.h5")
 
         except:
             print("Error: pd and h5 files were not found, check path")
 
-
-
     def plot_overlayedEIC(self,rawdatas,mz,rt_start,rt_end,alpha=0.3):
+        """
+        Plot an overlayed EIC for specified samples and mz and retention time range
+        @param rawdatas: list of rawData objects, samples to plot EIC for
+        @param mz: float, m/z value to extract EIC
+        @param rt_start: float, retention time value that is the starting value to plot
+        @param rt_end: float, retention time value that is the ending value to plot
+        @param alpha: float, transparency factor (0-1)
+        @return: None
+        """
         ts = np.linspace(rt_start,rt_end,self.resolution)
         for data in rawdatas:
             s = data.interpolate_data(mz,rt_start,rt_end)
             ints  = [np.max([x,0]) for x in s(ts)]
             plt.plot(ts,ints,alpha=alpha)
 
 
     @staticmethod
     def getNormalizedIntensityVector(data,mzs,rtstarts,rtends,resolution,q=None):
+        """
+        Get a list of EIC vectors from a single sample
+        @param data: rawData, rawData object to extract EICs for
+        @param mzs: list, list of m/z values to get EICs for
+        @param rtstarts: list, of retention times values that are the lower bound of the EIC window
+        @param rtends: list, of retention times values that are the upper bound of the EIC window
+        @param resolution: int, number of data points to sample in the EIC window
+        @param q: Queue or None, only used for multiprocessing
+        @return: numpy array, array of EICs (one row per EIC)
+        """
         out = np.zeros((len(mzs),resolution))
         i=0
         for mz,rt_start,rt_end in zip(mzs,rtstarts,rtends):
             s = data.interpolate_data(mz,rt_start,rt_end)
             out[i,:] = s(np.linspace(rt_start,rt_end,resolution))
             i += 1
         if type(q) != type(None):
             q.put(0)
         return out
 
     def makeDataMatrix(self,rawdatas,mzs,rts,align=False):
+        """
+        make a matrix of EICs that is composed of every EIC for each feature in each file
+        @param rawdatas: list of rawData objects, samples to generate EICs from
+        @param mzs: list, list of m/z values to get EICs for
+        @param rts: list,  list of retention time values to get EICs for
+        @param align: bool, whether to perform retention time alignment or not (True = align, False = do not align)
+        @return: numpy matrix, matrix of EICs. The order of the matrix is first by samples then by features. For example, for an ouput matrix generated from n samples and m features, would have length n * m and the EIC for the ith feature for the jth sample would be in row: i + (j * m)
+        """
+        #gather start and end times of EIC windows
         rtstarts = [rt - self.windowSize/2 for rt in rts]
         rtends = [rt + self.windowSize/2 for rt in rts]
+
+        #gather arguments for function
         args = []
         featInds = []
         for rawdata in rawdatas:
             featInds += list(range(len(mzs)))
             args.append([rawdata, mzs, rtstarts, rtends,self.resolution])
 
+        #get EICs
         result = startConcurrentTask(PeakDetective.getNormalizedIntensityVector, args, self.numCores, "forming matrix", len(args))
 
+        #concatenate EICs
         result = np.concatenate(result,axis=0)
 
+        #align EICs
         if align:
             result = alignDataMatrix(result,featInds,True,self.numCores)
 
         return result
 
-    def generateGaussianPeaks(self,n, centerDist, numPeaksDist=(0,2), widthFactor=0.1, heightFactor=1):
-        X_signal = np.zeros((n,self.resolution)) #self.generateNoisePeaks(X_norm, tics)
-        switcher = list(range(len(centerDist)))
-        for x, s in zip(range(len(X_signal)), np.random.random(len(X_signal))):
-            if numPeaksDist[0] >= numPeaksDist[1]:
-                numGuass = numPeaksDist[0]
-            else:
-                numGuass = np.random.randint(numPeaksDist[0], numPeaksDist[1])
-            for _ in range(numGuass):
-                ind = int(np.random.choice(switcher))
-                X_signal[x] += heightFactor * stats.norm.pdf(np.linspace(0, 1, self.resolution),
-                                     stats.uniform.rvs(centerDist[ind][0], centerDist[ind][1] - centerDist[ind][0]),
-                                     widthFactor * s + .001)
-            #if np.sum(tmp) > 0:
-            #    tmp = (1 - s2n[x]) * tmp / np.sum(tmp)
-        X_signal = normalizeMatrix(X_signal)
-
-        return X_signal
-
-    def generateFalsePeaks(self,peaks,raw_datas, n=None,align=False):
-        if type(n) == type(None):
-            n = len(peaks)
-
-        peaks_rand = pd.DataFrame()
-        peaks_rand["rt"] = rd.choices(list(peaks["rt"].values),k=n)
-        peaks_rand["mz"] = rd.choices(list(peaks["mz"].values),k=n)
-
-        X_noise = self.makeDataMatrix(raw_datas,peaks_rand["mz"].values,peaks_rand["rt"].values,align)
-
-        return X_noise
-
-    def generateSignalPeaks(self,peaks,raw_datas,widthFactor = 0.1,heightFactor = 1,n=None,align=False):
-        if type(n) == type(None):
-            n = len(peaks)
-        X_noise = self.generateFalsePeaks(peaks,raw_datas,n=n,align=align)
-        X_signal = self.generateGaussianPeaks(int(n*len(raw_datas)),[[0.45,0.5],[0.5,0.55]],(1,1),widthFactor,heightFactor)
-
-        samp = peaks.loc[rd.choices(list(peaks.index.values),k=int(np.ceil(n))),:]
-        mzs = list(samp["mz"].values)
-
-        tmp = self.makeDataMatrix(raw_datas,mzs,samp["rt"].values,align=align)
-        tmp = tmp[:n*len(raw_datas),:]
-
-        signal_areas = np.array([integratePeak(x) for x in tmp])
-
-        X_signal = signal_areas[:, np.newaxis] * X_signal
-
-        X = X_noise + X_signal
-
-        return X
-
-
     def trainSmoother(self,peaks,raw_datas,numPeaks,smooth_epochs,batch_size,validation_split):
+        """
+        Train smoothing autoencoder network
+        @param peaks: Pandas DataFrame, list of features detected from some peak detection software
+        @param raw_datas: list of rawData objects, samples to use for training
+        @param numPeaks: int, number of peaks to sample to train autoencoder
+        @param smooth_epochs: int, number of epochs to train for
+        @param batch_size: int, batch size for training
+        @param validation_split: float, fraction of EICs to hold out for validation, between 0-1.
+        @return: None
+        """
         #generate data matrix
         print("generating EICs...")
         mzs = rd.choices(list(peaks["mz"].values),k=int(numPeaks/len(raw_datas)))
         rts = rd.choices(list(peaks["rt"].values),k=int(numPeaks/len(raw_datas)))
 
         X = self.makeDataMatrix(raw_datas,mzs,rts)
 
@@ -277,74 +164,107 @@
         print("done")
 
         #fit autoencoder
         print("fitting smoother...")
         smoother = Smoother(self.resolution)
         smoother.fit(X_norm, X_norm, epochs=smooth_epochs, batch_size=batch_size, validation_split=validation_split,verbose=1)
 
+        #set updated models
         self.smoother = smoother
         self.encoder = keras.Model(smoother.input, smoother.layers[7].output)
         print("done")
 
     def trainClassifier(self,X,y,X_val,y_val,min_epochs,max_epochs,batch_size,restarts):
+        """
+        Train classifer network
+        @param X: numpy matrix, input EICs to train on
+        @param y: numpy matrix, input labels to train on
+        @param X_val: numpy matrix, EICs to use a validation data
+        @param y_val: numpy matrix, input labels to use as validation
+        @param min_epochs: int, minimum number of epochs to train
+        @param max_epochs: int, maximum number of epochs to train
+        @param batch_size: int, batch size to use when training
+        @param restarts: int, number of random restarts to run
+        @return: EarlyStopping callback, training history in keras callback object
+        """
 
+        #normalize matrix
         X_norm = normalizeMatrix(X)
+
+        #calculate peak areas
         tics = np.log10(np.array([np.max([2, integratePeak(x)]) for x in X]))
+
+        #get latent rep. of EICs
         X_latent = self.encoder.predict(X_norm)
 
+        #normalize validation EICs
         X_tmp = normalizeMatrix(X_val)
+
+        #get peak areas for validation data
         tic_val = np.log10(np.array([np.max([2, integratePeak(x)]) for x in X_val]))
+
+        #get latent rep. of validaiton EICs
         X_val = self.encoder.predict(X_tmp)
 
 
+        #begin training
         bestLoss = np.inf
         bestWeights = -1
         bestValErr = -1
         bestBestEpoch = -1
         trainErr = -1
         trainLoss = -1
 
+        #iterate over random restarts
         for x in range(restarts):
 
+            #make callback object
             cb = keras.callbacks.EarlyStopping(
                 monitor="val_loss",
                 min_delta=0,
                 patience=3,
                 verbose=0,
                 mode="auto",
                 baseline=None,
                 restore_best_weights=True,
             )
 
             history = keras.callbacks.History()
 
+            # initialize classifier
             classifer = ClassifierLatent(X_latent.shape[1])
 
+            #train to minimum epochs
             if min_epochs > 0:
                 classifer.fit([X_latent,tics],y,epochs=int(min_epochs),batch_size=batch_size,verbose=0,
                               validation_data=([X_val, tic_val], y_val))
 
+            #train until maximum epochs with early stopping
             classifer.fit([X_latent, tics], y, epochs=int(max_epochs-min_epochs),
                           batch_size=batch_size, verbose=0, callbacks=[cb, history],
                           validation_data=([X_val, tic_val], y_val))
 
+            #get performance
             valLoss = history.history["val_loss"][cb.best_epoch]
             valErr = history.history["val_mean_absolute_error"][cb.best_epoch]
             bestEpoch = cb.best_epoch
 
-
+            #update best performers
             if valLoss < bestLoss:
                 bestLoss = valLoss
                 bestWeights = classifer.get_weights()
                 bestValErr = valErr
                 bestBestEpoch = bestEpoch
                 trainLoss = history.history["loss"][cb.best_epoch]
                 trainErr = history.history["mean_absolute_error"][cb.best_epoch]
+
+        #print performance
         print("loss:",trainLoss,"mean_absolute_error:",trainErr,"val loss:", bestLoss, "val_mean_absolute_error:",bestValErr, "numEpochs:", min_epochs + bestBestEpoch)
 
+        #set best weights
         classifer.set_weights(bestWeights)
 
         self.classifier = classifer
 
         return history
 
     def trainClassifierActive(self,X,X_labeled,y_labeled,min_epochs,max_epochs,batch_size,restarts,numVal = 10,numManualPerRound=3,inJupyter=True):
@@ -359,41 +279,53 @@
         y_val = np.zeros((numVal,2))
 
         X = X[[x for x in range(len(X)) if x not in valInds]]
 
         updatingInds = list(range(len(X)))
 
         for ind in range(len(X_val)):
-            val = self.labelPeak([X_val[ind]], 0, self.windowSize, inJupyter,"")
+            val = self.labelPeak([X_val[ind]], -1*self.windowSize/2, self.windowSize/2, inJupyter,"","relative retention time")
             y_val[ind, 0] = 1 - val
             y_val[ind, 1] = val
 
 
         if len(X_labeled) > 0:
             self.trainClassifier(X_labeled,
                                  y_labeled,
                                  X_val,y_val, min_epochs,max_epochs, batch_size, restarts)
 
         y[updatingInds] = self.classifyMatrix(X[updatingInds])
 
         doMore = True
         i=0
+
+        def padVal(val):
+            if val < 0.5:
+                return val + 1e-8
+            else:
+                return val - 1e-8
+
         while doMore:
             if len(updatingInds) > 0:
 
-                entropies = [-1 * np.sum([yyy * np.log(yyy) for yyy in yy]) for yy in y[updatingInds]]
+                entropies = [-1 * np.sum([padVal(val) * np.log(padVal(val)) for yyy in yy]) for yy in y[updatingInds]]
+
                 order = list(range(len(updatingInds)))
                 order.sort(key=lambda x: entropies[x], reverse=True)
                 order = [updatingInds[x] for x in order]
 
                 if len(order) < numManualPerRound:
                     numManualPerRound = len(order)
 
-                for ind in order[:numManualPerRound]:
-                    val = self.labelPeak([X[ind]], 0, self.windowSize, inJupyter, y[ind][1])
+                inds = np.random.choice(order,numManualPerRound,replace=False,p=np.array(entropies) / np.sum(entropies))
+
+                #inds = order[:numManualPerRound]
+
+                for ind in inds:
+                    val = self.labelPeak([X[ind]], -1*self.windowSize/2, self.windowSize/2, inJupyter, y[ind][1],"relative retention time")
                     y[ind, 0] = 1 - val
                     y[ind, 1] = val
                     trainingInds.append(ind)
                     updatingInds.remove(ind)
 
                 if len(X_labeled) > 0:
                     X_train = np.concatenate((X[trainingInds],X_labeled),axis=0)
@@ -579,40 +511,90 @@
 
         X = X[toKeep]
 
         peak_scores = peak_scores.loc[goodInds,:]
 
         peak_scores = peak_scores.reset_index()
 
-        print(len(peak_scores), " peaks found")
+        apex_rts = self.updateRT(peak_scores,[raw.filename for raw in rawDatas],X,cutoff)
+
+        peak_scores["rt"] = np.round(apex_rts,2)
+
+        apex_mzs = self.updateMz(peak_scores,rawDatas,cutoff)
+
+        peak_scores["mz"] = np.round(apex_mzs,7)
 
         peak_intensities = self.performIntegration(X, [raw.filename for raw in rawDatas], peak_scores, cutoff)
-        #for raw in rawDatas:
-        #    peak_intensities[raw.filename] = raw.integrateTargets(transitionLists[raw.filename])[raw.filename].values
+
+        peak_intensities = peak_intensities.drop_duplicates(["mz","rt"],keep="first")
+        peak_scores = peak_scores.drop_duplicates(["mz","rt"],keep="first")
+
+        print(len(peak_scores), " peaks found")
 
         return peak_scores, peak_intensities, rois
 
+    def updateRT(self,peakScores,samples,X,cutoff,smooth=False):
+        i = 0
+        rts = []
+        dt = self.windowSize / self.resolution
+        for index, row in peakScores.iterrows():
+            inds = []
+            allInds = []
+            for n,samp in enumerate(samples):
+                ind = i + n * len(peakScores)
+                if row[samp] > cutoff:
+                    inds.append(ind)
+                allInds.append(ind)
+            if len(inds) > 0:
+                tmp = X[inds].sum(axis=0)
+                if smooth: tmp = self.smoother.predict(normalizeMatrix(np.array([tmp])), verbose=0)[0]
+                lb, rb, apex = findPeakBoundaries(tmp)
+
+            else:
+                apex = (self.resolution-1)/2
+
+            rt = (apex - (self.resolution-1)/2) * dt + row["rt"]
+            rts.append(rt)
+            i += 1
+            printProgressBar(i, len(peakScores), "refining retention times", printEnd="")
+
+        return rts
+
+    def updateMz(self,peak_scores,raw_data,cutoff):
+        mzs = []
+        i = 0
+        for index,row in peak_scores.iterrows():
+            tmp = []
+            for data in raw_data:
+                if row[data.filename] > cutoff:
+                    tmp.append(data.getApexMz(row["mz"],row["rt"]))
+            tmp = np.array(tmp)
+            mzs.append(np.average(tmp[:,0],weights=tmp[:,1]))
+            i += 1
+            printProgressBar(i, len(peak_scores), "refining mzs", printEnd="")
+        return mzs
+
     def label_peaks(self,raw_data,peaks,inJupyter = True):
         rt_starts = [row["rt"] - self.windowSize/2 for _,row in peaks.iterrows()]
         rt_ends = [row["rt"] + self.windowSize/2 for _,row in peaks.iterrows()]
         y = []
         mat = self.makeDataMatrix([raw_data],peaks["mz"].values,peaks['rt'])
         count = 1
         for vec,rt_start,rt_end in zip(mat,rt_starts,rt_ends):
-            y.append(self.labelPeak([vec],rt_start,rt_end,inJupyter,str(count) + "/" + str(len(mat))))
+            y.append(self.labelPeak([vec],rt_start,rt_end,inJupyter,str(count) + "/" + str(len(mat)),"retention time"))
             count += 1
         peaks["classification"] = y
         return peaks
 
-    def labelPeak(self,vecs,rt_start,rt_end,inJupyter,title=""):
+    def labelPeak(self,vecs,rt_start,rt_end,inJupyter,title="",xlabel="retention time"):
         plt.figure()
         plt.ion()
         xs = np.linspace(rt_start, rt_end, len(vecs[0]))
         [plt.plot(xs, vec) for vec in vecs]
-        plt.xlabel("time (arbitrary)")
+        plt.xlabel(xlabel)
         plt.ylabel("intensity")
         plt.title(title)
         plt.show(block=False)
         plt.pause(0.001)
         print("Enter classification (1=True Peak, 0=Artifact): ")
         val = input()
 
@@ -697,71 +679,14 @@
             for ind,sample in zip(allInds,samples):
                 peak_areas.at[index,sample] = integratePeak(X[ind],[lb,rb])
             i += 1
             printProgressBar(i, len(peakScores), "integrating peaks", printEnd="")
 
         return peak_areas
 
-def plotScoringStatistics(scores,labels):
-    tpr = []
-    fdr = []
-    cutoffs = np.linspace(0,1.0,100)
-    for cutoff in cutoffs:
-        fdr.append(1-met.precision_score(labels,scores > cutoff,zero_division=0))
-        tpr.append(met.recall_score(labels,scores>cutoff,zero_division=0))
-    plt.scatter(cutoffs,tpr,c="black",label="TPR")
-    plt.plot(cutoffs,tpr,c="black")
-
-    plt.scatter(cutoffs,fdr,c="red",label="FDR")
-    plt.plot(cutoffs,fdr,c="red")
-    plt.legend()
-    plt.xlabel("cutoff")
-    plt.ylabel("performance")
-
-
-def validateInput(input):
-    try:
-        input = float(input)
-        if input not in [0,1]:
-            return False
-        return True
-    except:
-        return False
-
-def binarySearchROI(poss, query,ppm):
-
-    if len(poss) == 0:
-        return False, 0
-
-    pos = bisect_left([x["mz_mean"] for x in poss], query)
-
-    if pos == len(poss):
-        if 1e6 * np.abs(query - poss[-1]["mz_mean"]) / query < ppm:
-            return True, pos - 1
-        else:
-            return False, pos
-    elif pos == 0:
-        if 1e6 * np.abs(query - poss[0]["mz_mean"]) / query < ppm:
-            return True, 0
-        else:
-            return False, pos
-    else:
-        ldiff = 1e6 * np.abs(query - poss[pos - 1]["mz_mean"]) / query
-        rdiff = 1e6 * np.abs(query - poss[pos]["mz_mean"]) / query
-
-        if ldiff < rdiff:
-            if ldiff < ppm:
-                return True, pos - 1
-            else:
-                return False, pos
-        else:
-            if rdiff < ppm:
-                return True, pos
-            else:
-                return False, pos
 
 class rawData():
     def __init__(self,data={},filename="",ppm=0,timestamp=None):
         self.data = data
         self.filename = filename
         self.rts = list(self.data.keys())
         self.rts.sort()
@@ -816,22 +741,35 @@
             ind = Origind - 1
             while ind > -1 and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end :
                 tmp += self.data[rt][ind][1]
                 ind -= 1
             intensity.append(tmp)
         return rts,intensity
 
-    # def integrateTargets(self,transitionList):
-    #     areas = []
-    #     for index,row in transitionList.iterrows():
-    #         rts,intensity = self.extractEIC(row["mz"],row["rt_start"],row["rt_end"])
-    #         area = np.trapz(intensity,rts)
-    #         areas.append(area)
-    #     transitionList[self.filename] = areas
-    #     return transitionList
+    def getApexMz(self,mz,rt):
+        width = self.ppm * mz / 1e6
+        mz_start = mz - width
+        mz_end = mz + width
+        rt = self.rts[getIndexOfClosestValue(self.rts,rt)]
+        highestMz = mz
+        highestIntensity = 1
+        Origind = getIndexOfClosestValue([x[0] for x in self.data[rt]], mz)
+        ind = int(Origind)
+        while ind < len(self.data[rt]) and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end:
+            if self.data[rt][ind][1] > highestIntensity:
+                highestIntensity = self.data[rt][ind][1]
+                highestMz = self.data[rt][ind][0]
+            ind += 1
+        ind = Origind - 1
+        while ind > -1 and self.data[rt][ind][0] > mz_start and self.data[rt][ind][0] < mz_end:
+            if self.data[rt][ind][1] > highestIntensity:
+                highestIntensity = self.data[rt][ind][1]
+                highestMz = self.data[rt][ind][0]
+            ind -= 1
+        return highestMz,highestIntensity
 
     def interpolate_data(self,mz,rt_start,rt_end):
         rts,intensity = self.extractEIC(mz,rt_start,rt_end)
         if len(rts) > 3:
             #smoothing = smoothing * len(rts) * np.max(intensity)
             #s = UnivariateSpline(rts,intensity,ext=1,s=smoothing)
             s = interp1d(rts,intensity,kind="linear",fill_value=0,bounds_error=False)
@@ -844,17 +782,14 @@
     def getMergedSpectrum(self,rtRange=None,intensityThresh=0,ppm=1):
         if rtRange is None:
             rtRange = [self.rts[0],self.rts[-1]]
         spectra = [[[mz,i] for mz,i in self.data[rt] if i > intensityThresh] for rt in self.rts if rt > rtRange[0] and rt < rtRange[1]]
         return mergeSpectra(spectra,ppm)
 
 
-
-
-
 def Smoother(resolution):
     # build autoencoder
     autoencoderInput = keras.Input(shape=(resolution,))
     x = layers.Reshape((resolution, 1))(autoencoderInput)
 
     kernelsize = 3
     stride = 1
@@ -1020,15 +955,15 @@
         peaks_norm = deepcopy(peaks)
 
     reference_peak = peaks_norm[reference]
     ref = list(range(len(reference_peak)))
 
     for x,peak in enumerate(peaks_norm):
         if x > 0:
-            distance, path = fastdtw(reference_peak, peak, dist=euclidean)
+            distance, path = fastdtw(np.array(reference_peak).flatten(), np.array(peak).flatten(), dist=2)
             xs = []
             ys = []
 
             prev = path[0][0]
             tmp = [peaks[x][path[0][1]]]
             for p1,p2 in path[1:]:
                 if p1 != prev:
@@ -1060,34 +995,14 @@
     result = startConcurrentTask(alignPeaks,args,numCores,"aligning EICs",len(uniquePeaks))
     for peaks,inds in zip(result,order):
         for peak,ind in zip(peaks,inds):
             matrix[ind] = peak
     return matrix
 
 
-# def isoLock(refMasses,queryMasses,driftRange=0.005,toTest=50,targetDiff=0.0001):
-#     bestDrift = 0
-#     bestIsoPairs = 0
-#     refMasses = list(refMasses)
-#     refMasses.sort()
-#
-#     for drift in np.linspace(-1*driftRange,driftRange,toTest):
-#         sep = 1.00336 + drift
-#         massesToFind = refMasses + sep
-#         numPairs = 0
-#         for m in massesToFind:
-#             best = take_closest(queryMasses,m)
-#             if np.abs(best-m) < targetDiff:
-#                 numPairs += 1
-#         if (numPairs == bestIsoPairs and drift < bestDrift) or numPairs > bestIsoPairs:
-#             bestDrift = drift
-#             bestIsoPairs = numPairs
-#     print(bestIsoPairs,"isopairs found with drift",bestDrift)
-#     return bestDrift
-
 def takeClosestInd(myList, myNumber):
     """
     Assumes myList is sorted. Returns closest value to myNumber.
 
     If two numbers are equally close, return the smallest number.
     """
 
@@ -1133,7 +1048,191 @@
     else:
         mergedSpectrumMzs = []
         mergedSpectrumInts = []
 
 
     return [[mz,i] for mz,i in zip(mergedSpectrumMzs,mergedSpectrumInts)]
 
+#Utility functions:
+
+#runs a function concurently.
+def startConcurrentTask(task,args,numCores,message,total,chunksize="none",verbose=True):
+
+    if verbose:
+        m = Manager()
+        q = m.Queue()
+        args = [a + [q] for a in args]
+        t = Thread(target=updateProgress, args=(q, total, message))
+        t.start()
+    if numCores > 1:
+        p = Pool(numCores)
+        if chunksize == "none":
+            res = p.starmap(task, args)
+        else:
+            res = p.starmap(task, args, chunksize=chunksize)
+        p.close()
+        p.join()
+    else:
+        res = [task(*a) for a in args]
+    if verbose: t.join()
+    return res
+
+
+def safeNormalize(x):
+    """
+    Safely normalize a vector, x, to sum to 1.0. If x is the zero vector return the normalized unity vector
+    """
+    if np.sum(x) < 1e-6:
+        tmp = np.ones(x.shape)
+        return tmp / np.sum(tmp)
+    else:
+        return x/np.sum(x)
+
+def normalizeMatrix(X):
+    """
+    Normalize a matrix so that the rows of X sum to one
+    """
+    return np.array([safeNormalize(x) for x in X])
+
+def classify(preds):
+    """
+    Classify predictions, preds, by returning the index of the highest scoring class
+    """
+    classes = np.zeros(preds.shape)
+    for x in range(len(preds)):
+        classes[x,list(preds[x]).index(np.max(list(preds[x])))] = 1
+    return classes
+
+
+def take_closest(myList, myNumber):
+    """
+    Assumes myList is sorted. Returns closest value to myNumber.
+
+    If two numbers are equally close, return the smallest number.
+    """
+    pos = bisect_left(myList, myNumber)
+    if pos == 0:
+        return myList[0]
+    if pos == len(myList):
+        return myList[-1]
+    before = myList[pos - 1]
+    after = myList[pos]
+    if after - myNumber < myNumber - before:
+        return after
+    else:
+        return before
+
+
+
+def printProgressBar(iteration, total, prefix='', suffix='', decimals=1, length=50, fill='█', printEnd="\r"):
+    """
+    Call in a loop to create terminal progress bar
+    @params:
+        iteration   - Required  : current iteration (Int)
+        total       - Required  : total iterations (Int)
+        prefix      - Optional  : prefix string (Str)
+        suffix      - Optional  : suffix string (Str)
+        decimals    - Optional  : positive number of decimals in percent complete (Int)
+        length      - Optional  : character length of bar (Int)
+        fill        - Optional  : bar fill character (Str)
+        printEnd    - Optional  : end character (e.g. "\r", "\r\n") (Str)
+    """
+    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
+    filledLength = int(length * iteration // total)
+    bar = fill * filledLength + '-' * (length - filledLength)
+    print(f'\r{prefix} |{bar}| {percent}% {suffix}', end=printEnd)
+    # Print New Line on Complete
+    if iteration == total:
+        print()
+
+def updateProgress(q, total,message = ""):
+    """
+    update progress bar
+    """
+    counter = 0
+    while counter != total:
+        if not q.empty():
+            q.get()
+            counter += 1
+            #if counter % 20 == 0:
+            printProgressBar(counter, total,prefix = message, printEnd="")
+
+
+def getIndexOfClosestValue(l,v):
+    """
+    get index of list with closest value to v, assumes l is sorted
+    """
+    pos = bisect_left(l, v)
+    if pos == 0:
+        return 0
+    if pos == len(l):
+        return pos - 1
+    before = l[pos - 1]
+    after = l[pos]
+    if after - v < v - before:
+        return pos
+    else:
+        return pos - 1
+
+def plotScoringStatistics(scores, labels):
+    tpr = []
+    fdr = []
+    cutoffs = np.linspace(0, 1.0, 100)
+    for cutoff in cutoffs:
+        fdr.append(1 - met.precision_score(labels, scores > cutoff, zero_division=0))
+        tpr.append(met.recall_score(labels, scores > cutoff, zero_division=0))
+    plt.scatter(cutoffs, tpr, c="black", label="TPR")
+    plt.plot(cutoffs, tpr, c="black")
+
+    plt.scatter(cutoffs, fdr, c="red", label="FDR")
+    plt.plot(cutoffs, fdr, c="red")
+    plt.legend()
+    plt.xlabel("cutoff")
+    plt.ylabel("performance")
+
+def validateInput(input):
+    """
+    Validate input, used for the labelPeaks() function
+    @param input: str, user input
+    @return: Bool, True = user input was a 0 or 1, False otherwise
+    """
+    try:
+        input = float(input)
+        if input not in [0, 1]:
+            return False
+        return True
+    except:
+        return False
+
+def binarySearchROI(poss, query, ppm):
+    """
+    Search function used in ROI calculations
+    """
+    if len(poss) == 0:
+        return False, 0
+
+    pos = bisect_left([x["mz_mean"] for x in poss], query)
+
+    if pos == len(poss):
+        if 1e6 * np.abs(query - poss[-1]["mz_mean"]) / query < ppm:
+            return True, pos - 1
+        else:
+            return False, pos
+    elif pos == 0:
+        if 1e6 * np.abs(query - poss[0]["mz_mean"]) / query < ppm:
+            return True, 0
+        else:
+            return False, pos
+    else:
+        ldiff = 1e6 * np.abs(query - poss[pos - 1]["mz_mean"]) / query
+        rdiff = 1e6 * np.abs(query - poss[pos]["mz_mean"]) / query
+
+        if ldiff < rdiff:
+            if ldiff < ppm:
+                return True, pos - 1
+            else:
+                return False, pos
+        else:
+            if rdiff < ppm:
+                return True, pos
+            else:
+                return False, pos
```

### Comparing `PeakDetective-0.1.4/PeakDetective/detection_helper.py` & `PeakDetective-0.1.6/PeakDetective/detection_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 import pandas as pd
 import scipy.stats as stats
 import os
 import uuid
 import bisect
 from . import printProgressBar, startConcurrentTask, getIndexOfClosestValue
+from sklearn.ensemble import RandomForestRegressor
+import matplotlib.pyplot as plt
+
 
 class PeakList():
     def __init__(self,peakList = None):
         if type(peakList) == type(None):
             self.peakList = pd.DataFrame()
         else:
             self.peakList = peakList
@@ -160,14 +163,31 @@
 
 
         self.peakList[sample_keys] = data_imp.transpose()
 
     def logTransform(self,sampleCols):
         self.peakList[sampleCols] = np.log2(self.peakList[sampleCols].values)
 
+    def batchCorrect(self,sampleCols,qcCols,batchInfo,plot=True):
+
+        reg = RandomForestRegressor(n_jobs=10)
+
+        peak_areas = self.peakList[sampleCols].values.transpose()
+
+        X = np.array(batchInfo[qcCols])
+        y = peak_areas[qcCols] - np.mean(peak_areas[qcCols], axis=0)
+        reg.fit(X, y)
+        preds = reg.predict(batchInfo)
+        if plot:
+            plt.figure()
+            plt.plot(list(range(len(preds))),np.mean(preds,axis=1))
+            plt.errorbar(list(range(len(preds))),np.mean(preds,axis=1),yerr=np.std(preds,axis=1),fmt=".",capsize=1)
+            plt.xlabel("run order")
+            plt.ylabel("correction factor")
+        self.peakList[sampleCols] = np.array(peak_areas - preds).transpose()
 
         
 
 def compareRT(feat1,feat2,rtTol):
 
     rt1 = feat1["rt"]
     rt2 = feat2["rt"]
@@ -177,43 +197,50 @@
         
     return False
 
 def mergePeakLists(peakLists,names,ppm=20,rtTol=.5):
     peakLists = [x[["mz","rt"]].reset_index() for x in peakLists]
     mergedList = peakLists[0]
     peakFounders = {n:{} for n in names}
+    peakIndices = {n:{} for n in names}
 
     for index,row in mergedList.iterrows():
         peakFounders[names[0]][index] = 1
+        peakIndices[names[0]][index] = index
         for n in names[1:]:
             peakFounders[n][index] = 0
-
+            peakIndices[n][index] = -1
     for x,n in zip(peakLists[1:],names[1:]):
         for index,row in x.iterrows():
             new = True
             mz_bounds = [row["mz"] - ppm*row["mz"]/1e6,row["mz"] + ppm*row["mz"]/1e6]
             if len(mergedList) > 0:
                 filt = mergedList[(mergedList["mz"] > mz_bounds[0]) & (mergedList["mz"] < mz_bounds[1])]            
                 for index2,row2 in filt.iterrows():
                     if compareRT(row,row2,rtTol):
                         new = False
-                        peakFounders[n][index2] = 1 
+                        peakFounders[n][index2] = 1
+                        peakIndices[n][index2] = index
                         break
             if new:
                 ind = len(mergedList)
                 mergedList = pd.concat((mergedList,x.iloc[index:index+1,:]),axis=0,ignore_index=True)
                 for n2 in names:
                     peakFounders[n2][ind] = 0
+                    peakIndices[n2][ind] = -1
+
                 peakFounders[n][ind] = 1
+                peakIndices[n][ind] = index
                 
       
                             
     peakFounders = pd.DataFrame.from_dict(peakFounders,orient="index").transpose()
-    mergedList = pd.concat((mergedList,peakFounders),axis=1,ignore_index=False)
-    return mergedList
+    peakIndices = pd.DataFrame.from_dict(peakIndices,orient="index").transpose()
+
+    return pd.concat((mergedList,peakFounders),axis=1,ignore_index=False),pd.concat((mergedList,peakIndices),axis=1,ignore_index=False)
 
 def runMzUnity(df,polarity,ppm,q=None):
     dir = os.path.dirname(__file__)
     path = str(uuid.uuid4()) + ".csv"
     if len(df) > 1:
         df.to_csv(path)
         os.system("Rscript " + os.path.join(dir, "mz_unity.R") + " " + path + " " + str(polarity) + " " + str(ppm) + " " + path)
```

### Comparing `PeakDetective-0.1.4/PeakDetective/find_peaks.R` & `PeakDetective-0.1.6/PeakDetective/find_peaks.R`

 * *Files identical despite different names*

### Comparing `PeakDetective-0.1.4/PeakDetective/mz_unity.R` & `PeakDetective-0.1.6/PeakDetective/mz_unity.R`

 * *Files identical despite different names*

### Comparing `PeakDetective-0.1.4/PeakDetective.egg-info/PKG-INFO` & `PeakDetective-0.1.6/PeakDetective.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: PeakDetective
-Version: 0.1.4
+Version: 0.1.6
 Summary: Curates and detects LC/MS peaks in metabolomics datasets
 Home-page: https://github.com/e-stan/PeakDetective/
 Author: Ethan Stancliffe
 Author-email: estancl1234@gmail.com
 License: MIT
-Download-URL: https://github.com/e-stan/PeakDetective/archive/v0.1.4.tar.gz
+Download-URL: https://github.com/e-stan/PeakDetective/archive/v0.1.6.tar.gz
 Description: UNKNOWN
 Keywords: Metabolomics,LC/MS,Deep Learning,semi-supervised learning,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PeakDetective-0.1.4/setup.py` & `PeakDetective-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PeakDetective',  # How you named your package folder (MyLib)
     packages=["PeakDetective"],  # Chose the same as "name"
-    version='0.1.4',  # Start with a small number and increase it with every change you make
+    version='0.1.6',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Curates and detects LC/MS peaks in metabolomics datasets',  # Give a short description about your library
     author='Ethan Stancliffe',  # Type in your name
     author_email='estancl1234@gmail.com',  # Type in your E-Mail
     url='https://github.com/e-stan/PeakDetective/',  # Provide either the link to your github or to your website
-    download_url='https://github.com/e-stan/PeakDetective/archive/v0.1.4.tar.gz',  # I explain this later on
+    download_url='https://github.com/e-stan/PeakDetective/archive/v0.1.6.tar.gz',  # I explain this later on
     keywords=['Metabolomics', 'LC/MS', "Deep Learning","semi-supervised learning","machine learning"],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'pyteomics',
         'numpy',
         'scipy',
         "matplotlib",
         "tensorflow",
```

