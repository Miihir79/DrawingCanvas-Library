# DrawingCanvas
library for drawing app canvas
> Step 1.Add this dependency to your build.gradle (project) file

```gradle
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  ```
 >Step 2. Add the dependency to your build.gradle(app) file
 
 ```gradle
 dependencies {
	        implementation 'com.github.Miihir79:DrawingCanvas:1.0.1'
	}
  ```
  
  >Step 3. Add the XML code 
  
  ```XML
  <com.mihir.drawingcanvas.drawingView
        android:id="@+id/drawing_view"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent">

    </com.mihir.drawingcanvas.drawingView>
```

>Step 4. Refrence the canvas in XML to use it's functions

```
    drawing_view.setBrushAlpha(120)// values from 0-255
    drawing_view.setBrushColor(R.color.white) 
    drawing_view.setSizeForBrush(12) // takes value from 0-35
        
```
