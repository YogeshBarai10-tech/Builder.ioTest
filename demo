// 1. This is your main app logic
useStore({
  searchValue: "",
  isMenuOpen: false,
  signInHovered: false,
  signInPressed: false,
  signUpHovered: false,
  signUpPressed: false,

  handleSearch() {
    console.log("Searching for:", state.searchValue);
  },
  toggleMenu() {
    state.isMenuOpen = !state.isMenuOpen;
  },
  handleSignIn() {
    console.log("Sign In clicked");
  },
  handleSignUp() {
    console.log("Sign Up clicked");
  },
  handleKeyDown(event, action) {
    if (event.key === "Enter" || event.key === " ") {
      event.preventDefault();
      action();
    }
  }
});

// 2. Define the Translate function globally
window.googleTranslateElementInit = function () {
  new google.translate.TranslateElement({
    pageLanguage: 'en',
    includedLanguages: 'hi,fr,es,de', // Add more language codes as needed
    layout: google.translate.TranslateElement.InlineLayout.SIMPLE
  }, 'google_translate_element');
};

// 3. Load Google Translate script
const script = document.createElement('script');
console.log('work');
script.src = 'https://translate.google.com/translate_a/element.js?cb=googleTranslateElementInit';
console.log(script);
document.body.appendChild(script);
