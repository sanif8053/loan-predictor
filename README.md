# loan-predictor
A Python Based Data science Project in which Loan Status was predict that a person should given a loan or not, based on some attributes.In the project Bayesian, Decision Tree, Random forest, Knn, Logistic Regression and Random Forest models Were applied. K-fold Data spliting approach was used for Data cross validation. 
```yaml
workflows:
  primary:
    steps:
    #...
    # use one of the following build step as per  your requirement
    #To generate .app file
    -  Xcode build for simulator: {}
    #To generate .ipa file
    - Xcode Archive & Export for iOS: {} 
    #To generate .apk file
    - android-build: {} 
    - sofy-upload:
      inputs:
      #choose one of the following variable as per your above choice of build step
      - build_path: $SOFY_APK_PATH (Android build), $BITRISE_IPA_PATH (Xcode Archive & Export for iOS), $BITRISE_APP_DIR_PATH (Xcode build for simulator)
      - subscription_key: 80b30c4e-c920-40a7-9682-6ad2e779a67f #from your secrets
    #...
        
```
