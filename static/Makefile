build:
	@echo "Building customer.less..."
	@cp -f src/img/*.*  img/
	@recess --compile src/css/customer.less > css/tmp_customer.css
	@spritemapper css/tmp_customer.css
	@mv css/customer-sprite.png img/customer-sprite.png
	@recess --compress css/customer.css > css/tmp_customer.css
	@mv -f css/tmp_customer.css css/customer.css
	@echo "Build Success."