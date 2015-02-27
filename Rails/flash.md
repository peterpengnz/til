## Flash messages

The flash is a special part of the session which is cleared with each request.
This means that values stored there will only be available in the next request, which is useful for passing error messages etc.

Checkout (Rails API)[http://api.rubyonrails.org/classes/ActionDispatch/Flash/FlashHash.html]

Good to know the `now` method and also `discard` and `keep` methods.
