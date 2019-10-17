# rails_note
<br>
## CSRF 오류 발생시 (ActionController::InvalidAuthenticityToken)
<br>
  class ApplicationController < ActionController::Base
	  skip_before_action :verify_authenticity_token, raise: false
  end


