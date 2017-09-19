# notesReactNative
Information for my references

<br />
react-navigation@1.0.0-beta.12 <br />
react-native@0.42.0 <br />
react-redux@5.0.5 <br />

<br /><br />

1) static navigationOptions cannot access directly to redux props.

solution: 
- inside componentDidMount call setParams for navigation. <br />
  this.props.navigation.setParams({ something: this.props.something }) 
- inside static navigationOptions call navigation params to use the props <br />
  navigation.state.params.something()
  
<br /><br />
