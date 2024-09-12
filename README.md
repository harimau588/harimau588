import React, {Componen} from 'react';
import {
 StlyeSheet, Text, View, StatusBar, Touchableopacity
} from 'react-native';
import logo from '../component/Logo';
import From from'../component/From';
import {Action} from 'react-native-rourter-flux';
export defaul class Login extends Componen<{}> {
signup(){
Action.signup()
}

render(){
return(
<View style = {style.container}>
<logo/>
<From type = "Login"/>
<View style = {style.signupTextCont}>
<Text style = {style.signupText}> Anda Belum Punya Akun ? </Text>
<Touchableopacity onPres = {this.signup}>
<Text style = {style.signupButton}> Signup </Text></Touchableopacity>
<View></View
)
}}
const style = StyleSheet.create({
container : {
backgroundColor : '455a64', flex : 1, alignItem : 'center',
justifyContent : {
}, signupTextCont : {
flexGrow : 1, alignItem : 'flex-end', justifyContent : 'center'
paddingVartical : 16, flexDirection : 'row'
},
signupText : {
color : 'rgba(225,225,225,0.6)', fontSize : 16
},
signupButton : {
color : '#ffffff', fontsize : 16, fontweight : '500'
}
});

