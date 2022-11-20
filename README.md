# REACTNATIIVE
a small sign up page 


import {View, Text ,StyleSheet , Button ,Alert, TextInput, Image, ScrollView,SafeAreaView } from 'react-native'
import React,{useState} from 'react'
 

export default function App (){
  const [name, onChangeText] =useState()
  const [mobileNumber, onChangeNumber] =useState()

return (
  <SafeAreaView>
 <ScrollView>
  <View style={styles.body}>
  

    <Text style={styles.enter1}>Enter your "DETAILS TO REGISTER":</Text>

    <Image  source={{uri: '/Users/apple/Downloads/KWESI DAIN.jpeg'}}
    style={styles.image}
    
    />

    <Text style={styles.Name}>Please enter your name : </Text>

    <TextInput
        style={styles.input}
        onChangeText={onChangeText}
        value={Text}
        
    />
    <Text style={styles.Number}>Please enter your mobile Number :</Text>

    <TextInput
        style={styles.input}
        onChangeText={onChangeNumber}
        value={Number}
        
    />
    

    <Text style={styles.text}>My name is {name} and my mobile number is {mobileNumber} .</Text>

    <Text style={styles.text1}></Text>

    <Button title="Click here to REGISTER" backgroundColor="" onPress={ () => Alert.alert("YOU HAVE BEING REGISTERED")} 

    />
    
    
    
  </View>
  </ScrollView>
  </SafeAreaView>
  
  


  
  
  
)
}
const styles =StyleSheet.create({

  body:{
    flex:2,
    backgroundColor: "white",
    alignItems:"center",
    justifyContent:"center",
    marginHorizontal: 0,
    marginVertical:0,
    marginBottom: 0,
    marginLeft:0

    
  },

  text1:{
    fontSize: 40,
    margin: 70,
    color : "green",
    alignItems: "center",
    backgroundColor:"yellow",
    fontWeight:"bold"
   
  },

  image:{
    width : 200,
    height: 200,
    borderBottomEndRadius: 100,
    borderBottomLeftRadius:100,
    borderBottomRightRadius:100,
    borderTopRightRadius:100, 
    borderTopLeftRadius: 100,

  },

  text:{
    color:"black",
    margin:20,
    fontSize:17,
    fontStyle: "normal",
    justifyContent : "space-evenly",
   
    
  },

  input:{
    borderColor : "blue",
    borderWidth : 3,
    borderBottomEndRadius: 15,
    borderBottomLeftRadius:15,
    borderBottomRightRadius:15,
    borderTopRightRadius:15, 
    borderTopLeftRadius: 15,
    padding: 11,
    margin:10,
    width: 175,
  },
  
  enter1:{
    alignContent: "center",
    padding:30,
    marginEnd:120,
    justifyContent:"center",
    fontSize:17,
    fontWeight: "bold",
    textAlign: "left", 
  },

  Name:{
    fontSize:17,

  },
 
  Number:{
    fontSize :17,
  },


})


  
