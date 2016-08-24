# SLPointKeyboard
自定义小数点的键盘

使用方法很简单

    SLNumberKeyboard *tNumberKb = [[SLNumberKeyboard alloc] init];
    
    UITextField *myText = [[UITextField alloc]initWithFrame:CGRectMake((self.view.frame.size.width-200)/2, 100, 200, 40)];
    myText.placeholder = @"自定义小数点的键盘";
    myText.clearButtonMode = UITextFieldViewModeWhileEditing;
    myText.textAlignment = NSTextAlignmentLeft;
    myText.layer.borderColor = [UIColor grayColor].CGColor;
    myText.layer.borderWidth = 1;
    myText.layer.masksToBounds = YES;
    myText.layer.cornerRadius = 4;
    [self.view addSubview:myText];
    myText.inputView = tNumberKb;
    
    tNumberKb.textFiled = myText;
    
这样就搞定了一个自定义小数点的键盘啦，是不是很快啊。
希望能帮助大家，谢谢！
