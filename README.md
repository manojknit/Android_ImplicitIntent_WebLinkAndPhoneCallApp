# Android app to demonstrate Implicit intent behaviour using Web link and phone call
####                                                                                                     By Manoj Kumar
## Introduction 
Android app to demonstrate Implicit intent behaviour using Web link and phone call.


## How to Run
1.	Prerequsit: Android Studio, some Java knowledge
2.	Download or clone project code and open in Android studio.
3.	Run in Nexus 5 emulator.


## Technologies Used
1.	Java.
2.	Android Studio


## Application Screenshots
#### Main Activity
<img src="images/Android Emulator - Nexus_5X_API_265554 2018-02-18 16-40-28.png">

#### WebLink Open.
<img src="images/Android Emulator - Nexus_5X_API_265554 2018-02-18 16-40-43.png">
<img src="images/Android Emulator - Nexus_5X_API_265554 2018-02-18 16-41-00.png">

#### Phone call global intent
<img src="images/Android Emulator - Nexus_5X_API_265554 2018-02-18 16-41-17.png">

## Code
```
   public void OnOpenURLClick(View view) {
        EditText e=(EditText)findViewById(R.id.txtUrl);
        String content = e.getText().toString();
        Intent implicit = new Intent(Intent.ACTION_VIEW, Uri.parse(content));
        startActivity(implicit);
    }
    public void OnRingClick(View view) {

        EditText e=(EditText)findViewById(R.id.txtPhone);
        String content = e.getText().toString();
        Intent implicit = new Intent(Intent.ACTION_VIEW, Uri.parse("tel:"+content));
        startActivity(implicit);
    }

```

## Thank You
Manoj Kumar
