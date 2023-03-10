# react-native-searchable-animated-dropdown





https://user-images.githubusercontent.com/76813201/222146478-11cb4f2d-c740-411a-9a5a-cd012f5882c7.mp4




This library will take array as input and create a dropdown based on it.
More details and properties below:

Properties:

| Property                      | Type           | Default                             | Description                                                |
| ----------------------------- | -------------- | ---------------------------         | ---------------------------------------------------------- |
| setSelectedValue (Required)   | Function       | null                                | Returns the selected value                                 |
| data (Required)               | array          | ["Demo1", "Demo2", "Demo3"]         | Array of values you want in your dropdown.                 |
| initialTitle                  | String         | --Select--                          | Placeholder                                                |
| mainView                      | ViewStyle      | defaultStyle                        | To change the view of main container                       |
| titleStyle                    | ViewStyle      | defaultStyle                        | To change the style of title(Option Selected)              |
| dropdownContainer             | ViewStyle      | defaultStyle                        | To change the style of dropdown container                  |
| dropdownItemContainer         | ViewStyle      | defaultStyle                        | To change the style of individual dropdown item container  |
| dropdownItemText              | ViewStyle      | defaultStyle                        | To change the style of dropdown text (i.e. Options)        |
| dropdownSelectedItemContainer | ViewStyle      | defaultStyle                        | To change the style of option container which is selected. |
| dropdownSelectedItemText      | ViewStyle      | defaultStyle                        | To change the style of text which is currently selected    |
| imagePath                     | imported image | 'down-arrow.png'                    | To change the icon of the dropdown                         |
| imageStyle                    | ViewStyle      | defaultStyle                        | To change the style of image                               |
| touchOpacity                  | integer        | 0.7                                 | To change touch opacity of component                       |
| searchIcon                    | imported image/Image Path | 'search.png'             | To change the icon of the search Icon                      |
| searchImageStyle              | Image Style               | defaultStyle             | To change the style of search Icon                         |
| searchContainer               | TextInput Style           | defaultStyle             | To change the style of search container                    |
| showSearch                    | Boolean                   | true                     | Show/Hide search bar                                       |
| searchPlaceholder             | String                    | Search                   | Search Placeholder                                         |
| duration                      | number                    | 800                      | To change duration of animation                            |
| bottomContainerHeight         | number                    | 200                      | To change the height of bottom container                   |
| showOverlay                   | boolean                   | true                     | Hide/Show Overlay                                          |
| overLayColor                  | color                     | `rgba(128,128,128,0.25)` | Change color of overlay                                    |



1. setSelectedValue (\*Required)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        // Property Code //
        setSelectedValue={setSelectedValue} />
        );

}
export default App;
```

2. data (\*Required)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}

        // Property Code //
        data={['Aadarsh', 'Vraj', 'Helly', 'Krupa', 'Niyanta', 'Nidhi', 'Heta']}

        );

}
export default App;
```

3. initialTitle (Optional)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}

        // Property Code //
        initialTitle="Select Option"
      />
        );

}
export default App;
```

![Output For initialTitle](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchInitialTitle.png)

4. mainView (Optional)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"

        // Property Code //
        mainView={{backgroundColor: 'skyblue', width: 300}}

      />
        );

}
export default App;
```

![Output For mainView](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchMainView.png)

5. titleStyle (Optional)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}

        // Property Code //
        titleStyle={{fontSize: 20, color: 'yellow'}}


      />
        );

}
export default App;
```

![Output For titleStyle](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchTitleStyle.png)

6. dropdownContainer (Optional)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}

        // Property Code //
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}

      />
        );

}
export default App;
```

![Output For dropdownContainer](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchDropdownContainer.png)

7. dropdownItemContainer (Optional)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}

        // Property Code //
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
      />
        );

}
export default App;
```

![Output For dropdownItemContainer](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/searchDropdownIconContainer.png)

8. dropdownItemText (Optional)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}

        // Property Code //
        dropdownItemText={{color: 'white', fontSize: 20}}

      />
        );

}
export default App;
```

![Output For dropdownItemText](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchDropdownIcontext.png)

9. dropdownSelectedItemContainer (Optional)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}

        // Property Code //
        dropdownSelectedItemContainer={styles.fromStylesheet}

      />
        );

}
export default App;


const styles = StyleSheet.create({
  fromStylesheet: {backgroundColor: 'purple', justifyContent: 'center'},
});
```

![Output For dropdownSelectedItemContainer](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchSelectedItemContainer.png)

10. dropdownSelectedItemText (Optional)

code:

```
function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}

        // Property Code //
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}

      />
        );

}
export default App;
```

![Output For dropdownSelectedItemText](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchDropdownSelectedItemText.png)

11. imagePath (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}

        // Property Code //
        imagePath={Icon}

      />
        );

}
export default App;
```

![Output For imagePath](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/searchImagePath.png)

12. imageStyle (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}

        // Property Code //
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}


      />
        );

}
export default App;
```

![Output For imageStyle](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchImageStyle.png)

13. touchOpacity (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}

        // Property code //
        touchOpacity={0.8}


      />
        );

}
export default App;
```
14. searchIcon (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        // Property code //

        searchIcon={require('./search2.png')}



      />
        );

}
export default App;
```

![Output For searchIcon](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/searchIcon.png)

15. searchImageStyle (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        searchIcon={require('./search2.png')}

        // Property code //

        searchImageStyle={{backgroundColor: 'red', right: 110}}



      />
        );

}
export default App;
```

![Output For searchImageStyle](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/SearchImageStyle.png)

16. searchContainer (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        searchIcon={require('./search2.png')}
        searchImageStyle={{backgroundColor: 'red', right: 110}}

        // Property code //
        searchContainer={{backgroundColor: 'gold'}}




      />
        );

}
export default App;
```

![Output For searchContainer](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/searchContainer.png)

17. showSearch (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        searchIcon={require('./search2.png')}
        searchImageStyle={{backgroundColor: 'red', right: 110}}
        searchContainer={{backgroundColor: 'gold'}}

        // Property code //
        showSearch={false}




      />
        );

}
export default App;
```

![Output For searchContainer](https://github.com/DipeshMajithia/react-native-searchable-array-dropdown/blob/main/screenshots/showSearch.png)

17. searchPlaceholder (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        searchIcon={require('./search2.png')}
        searchImageStyle={{backgroundColor: 'red', right: 110}}
        searchContainer={{backgroundColor: 'gold'}}
        showSearch={true}
        // Property code //

        searchPlaceholder="Search Here..."




      />
        );
}
export default App;
```

18. duration (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        searchIcon={require('./search2.png')}
        searchImageStyle={{backgroundColor: 'red', right: 110}}
        searchContainer={{backgroundColor: 'gold'}}
        showSearch={true}
        searchPlaceholder="Search Here..."
        
        
        // Property code //
        duration={1000}



      />
        );
}
export default App;
```

19. bottomContainerHeight (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        searchIcon={require('./search2.png')}
        searchImageStyle={{backgroundColor: 'red', right: 110}}
        searchContainer={{backgroundColor: 'gold'}}
        showSearch={true}
        searchPlaceholder="Search Here..."
        duration={1000}
        
        // Property code //
        bottomContainerHeight={400}



      />
        );
}
export default App;
```

20. showOverlay (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        searchIcon={require('./search2.png')}
        searchImageStyle={{backgroundColor: 'red', right: 110}}
        searchContainer={{backgroundColor: 'gold'}}
        showSearch={true}
        searchPlaceholder="Search Here..."
        duration={1000}
        bottomContainerHeight={400}

        // Property code //
        showOverlay={false}


      />
        );
}
export default App;
```

21. overLayColor (Optional)

code:

```

import Icon from './caret-down.png';

function App() {
  const [selectedValue, setSelectedValue] = useState('');
  return (
      <Dropdown
        setSelectedValue={setSelectedValue}
        data={['Item1', 'Item2', 'Item3', 'Item4', 'Item5', 'Item6', 'Item7']}
        initialTitle="Select Option"
        mainView={{backgroundColor: 'skyblue', width: 300}}
        titleStyle={{fontSize: 20, color: 'yellow'}}
        dropdownContainer={{
          backgroundColor: 'orange',
          alignSelf: 'center',
          width: 200,
        }}
        dropdownItemContainer={{
          backgroundColor: 'magenta',
          borderRadius: 30,
        }}
        dropdownItemText={{color: 'white', fontSize: 20}}
        dropdownSelectedItemContainer={styles.fromStylesheet}
        dropdownSelectedItemText={{color: 'white', fontSize: 20}}
        imagePath={Icon}
        imageStyle={{backgroundColor: 'pink', borderRadius: 20}}
        touchOpacity={0.8}
        searchIcon={require('./search2.png')}
        searchImageStyle={{backgroundColor: 'red', right: 110}}
        searchContainer={{backgroundColor: 'gold'}}
        showSearch={true}
        searchPlaceholder="Search Here..."
        duration={1000}
        bottomContainerHeight={400}
        showOverlay={false}
        
        // Property code //
        overLayColor={`rgba(255,255,255,0.5)`}
        


      />
        );
}
export default App;
```
