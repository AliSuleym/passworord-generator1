// Array of special characters to be included in password
var specialCharacters = [
  '@',
  '%',
  '+',
  '\\',
  '/',
  "'",
  '!',
  '#',
  '$',
  '^',
  '?',
  ':',
  ',',
  ')',
  '(',
  '}',
  '{',
  ']',
  '[',
  '~',
  '-',
  '_',
  '.'
];

// Array of numeric characters to be included in password
var numericCharacters = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9'];

// Array of lowercase characters to be included in password
var lowerCasedCharacters = [
  'a',
  'b',
  'c',
  'd',
  'e',
  'f',
  'g',
  'h',
  'i',
  'j',
  'k',
  'l',
  'm',
  'n',
  'o',
  'p',
  'q',
  'r',
  's',
  't',
  'u',
  'v',
  'w',
  'x',
  'y',
  'z'
];

// Array of uppercase characters to be included in password
var upperCasedCharacters = [
  'A',
  'B',
  'C',
  'D',
  'E',
  'F',
  'G',
  'H',
  'I',
  'J',
  'K',
  'L',
  'M',
  'N',
  'O',
  'P',
  'Q',
  'R',
  'S',
  'T',
  'U',
  'V',
  'W',
  'X',
  'Y',
  'Z'
];

var includedCharacters = [];
var passwordLength = 0;
var generatedPassword = "";

// Function to prompt user for password options
function getPasswordOptions() {

   includedCharacters = [];

   passwordLength = parseInt(prompt("How many characters do you want the password?"));

  /*Validations for the length of the password and avoid empty input*/

  if (isNaN(passwordLength) || passwordLength <  10 || passwordLength > 64){
    alert("The pasword must be between 10 and 64 characters")
  
    return false;
  }

  

  /* prompts to confirm what types of characters are to be included in the password and more validations*/

 
 if (confirm("Do you want to include Lowercase characters")){

 includedCharacters = includedCharacters.concat(lowerCasedCharacters);

 } 
 if (confirm("Do you want to include Uppercase characters")){

 includedCharacters = includedCharacters.concat(upperCasedCharacters);

 }
 
 if (confirm("Do you want to include numbers")){

  includedCharacters =  includedCharacters.concat(numericCharacters);

 }
  
 if (confirm("Do you want to include special characters")){

  includedCharacters = includedCharacters.concat(specialCharacters)

 }

 return true;

}

// Function for getting a random element from an array
function getRandom(arr) {
  var randomIndex =  Math.floor(Math.random() * arr.length);
  return arr[randomIndex]

}

// Function to generate password with user input
function generatePassword() {


  generatedPassword = "";

  // loops through the array of chosen characters and randomly chose characters until the password length is reached

 for(var i = 0; i < passwordLength; i++){

  var nextCharacter = getRandom(includedCharacters)

  generatedPassword += nextCharacter
 }

  return generatedPassword;
}

// Get references to the #generate element
var generateBtn = document.querySelector('#generate');

// Write password to the #password input
function writePassword() {

  var prompt = getPasswordOptions();
  var passwordText = document.querySelector('#password');

  if(prompt){
    
    var password = generatePassword();
    passwordText.value = password;
   
  
    
  } else{
    passwordText.value = "";
  }

  }

  console.log(includedCharacters)
  

// Add event listener to generate button
generateBtn.addEventListener('click', writePassword);