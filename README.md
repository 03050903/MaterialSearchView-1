# MaterialSearchView
Android SearchView based on Material Design guidelines. The MaterialSearchView will overlay a Toolbar or ActionBar as well as display a ListView for the user to show suggested or recent searches.

## Usage
To add the MaterialSearchView library to your Android Studio project, simply add the following gradle dependency:
```java
  compile 'br.com.mauker.materialsearchview:materialsearchview:1.0.2'
```

At this current moment, the library has not yet been released to JCenter so you must also reference the maven repo in your build.gradle file:
```java
  repositories {
      maven {
          url  "http://dl.bintray.com/mauker/maven"
      }
  }
```

This library is supported with a min SDK of 14.

## Interfaces
Currently there are two interfaces that you can use to instantiate listeners for:

- `OnQueryTextListener`: This interface handles either QueryTextChange or QueryTextSubmit events inside the MaterialSearchView.
- `SearchViewListener`: This interfaces handles the open or close events of the MaterialSearchView.

## Custom Attributes
A number of custom attributes can be applied to the MaterialSearchView inside of your XML layout:
- `searchBackground`: The background drawable for the view.
- `searchVoiceIcon`: The drawable resource for the voice search icon.
- `searchCloseIcon`: The drawable resource for the close search icon.
- `searchBackIcon`: The drawable resource for the back icon.
- `searchSuggestionBackground`: The background drawable for the suggestions ListView.
- `android:hint`: The hint that appears in the EditText of the search view.
- `android:textColor`: The text color of the EditText of the search view.
- `android:textColorHint`: The text color of the hint in the EditText of the search view.

## Sample
<img src='http://i.stack.imgur.com/JgK6M.gif' width='400' height='640' />

## Credits
This library was created by Maurício Pessoa with contributions from:
- [Adam McNeilly](http://adammcneilly.com)

This project was inspired by the [MaterialSearchView](https://github.com/krishnakapil/MaterialSeachView) library by krishnakapil.

## License
The MaterialSearchView library is available under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0).
