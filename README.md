# rails_note
<br>

## CSRF 오류 발생시 (ActionController::InvalidAuthenticityToken)
	
	#ApplicationController 에서 아래의 옵션을 넣어준다.
	
	class ApplicationController < ActionController::Base
		skip_before_action :verify_authenticity_token, raise: false
	end


