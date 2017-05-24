# 3DPhotos

/Users/iOS/Desktop/Swift/OC/3DPhotos/11359.gif

3D立体可旋转相册,3DPhotos,3D云相册,3D云标签

 [商城下载(App Store)：3D立体相册 ](https://itunes.apple.com/cn/app/3d%E7%AB%8B%E4%BD%93%E7%9B%B8%E5%86%8C-3d%E7%AB%8B%E4%BD%93%E9%85%B7%E7%82%AB%E8%87%AA%E8%BD%AC%E7%9B%B8%E5%86%8C/id1236619999?mt=8)


[简介说明 ](http://www.jianshu.com/p/282cfa8ff3d3)


     // 调用展示
    self.sphereView = [[YoungSphere alloc] initWithFrame:CGRectMake(20, 200, 340, 320)];

     NSMutableArray *array = [[NSMutableArray alloc] initWithCapacity:0];

    for (NSInteger i = 0; i < 30; i ++) {

    self.btn = [UIButton buttonWithType:UIButtonTypeSystem];

    [_btn setBackgroundImage:[UIImage imageNamed:@"dog"] forState:(UIControlStateNormal)];

    _btn.frame = CGRectMake(0, 0, 60, 60);

    [_btn addTarget:self action:@selector(buttonPressed:) forControlEvents:UIControlEventTouchUpInside];

    [array addObject:_btn];

     [_sphereView addSubview:_btn];

    }

    [_sphereView setCloudTags:array];

    _sphereView.backgroundColor = [UIColor whiteColor];
  
    [self.view addSubview:_sphereView];

当然里面的很多元素都是可以改动的，根据自己需要自己改动即可
这里用的是Button，你也可改为其他的，数量也可改动




