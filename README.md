SDCardSender
============

This is ACRA plugin for saving crush report to SDCard.
- crush report is printed /sdcard/bug.txt

## installation
- clone this repository
- import this repository your Eclipse project
- copy bin/sdcardsender.jar to your Android project's libs folder

## Usage

see [https://github.com/ACRA/acra/wiki/BasicSetup#setting-up-your-project](Setting-up your project).
However, it is described as below for `android.app.Application` class.

        public void onCreate() {
            super.onCreate();
    
            ACRA.init(this);
            SDCardSender yourSender = new SDCardSender();
            ACRA.getErrorReporter().setReportSender(yourSender);
        }


