# Kecilin Compress

![](https://avatars2.githubusercontent.com/u/54971865?s=400&u=f863fcc9f514994a89a91feb159220f99a6c33f8&v=4)

## Introduction

This class for compress image (File, Bitmap) android

## Code Samples

```Java
Kecilin.compress(new File("path")).asFile("destrinationPath", "Filename");
Kecilin.compress(new Bitmap()).asBitmap();
```

You can use asBitmpa() or asFile to make and output

```Java
Kecilin.asBitmap();
Kecilin.asFile("destrinationPath", "Filename");
Kecilin.asFile("destrinationPath");
```

## Code Video
```Java
KecilinVideo.compressVideoLow(inputPath, destPath, new KecilinVideo.CompressListener() {
                        @Override
                        public void onStart() {
                        }

                        @Override
                        public void onSuccess() {
                        }

                        @Override
                        public void onFail() {
                        }

                        @Override
                        public void onProgress(float percent) {
                        }
                    });
```

You can use Low Medium High for quality Compress Level
```Java
KecilinVideo.compressVideoLow();
KecilinVideo.compressVideoMedium();
KecilinVideo.compressVideoHigh();
```

## Installation Instructions

Step 1. Authorize JitPack and get your personal access token: <br><br>
Step 2. Add the token to $HOME/.gradle/gradle.properties 

```Gradle
authToken=q1q2w3we3e4r5rt5t56t6
```


Then use authToken as the username in your build.gradle:


```Gradle
 allprojects {
    repositories {
        ...
        maven {
            url "https://jitpack.io"
            credentials { username authToken }
        }
    }
 }
```


Step 3. (Optional) You may need to approve JitPack Application on GitHub

Step 4. Add the dependency

```Gradle
	dependencies {
	        implementation 'com.github.Kecilin:Compress:v1.0'
	}
```


More Details for import project check [this](https://jitpack.io/private#auth)
