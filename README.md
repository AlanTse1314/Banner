# Banner

<com.alan.banner.Banner
     android:id="@+id/banner"
     android:layout_width="match_parent"
     android:layout_height="match_parent" />
     
     
     
     Banner banner = findViewById(R.id.banner);
        banner.setOnBannerListener(new OnBannerClickListener() {

            /**
             * 点击事件
             *
             * @param bannerBean 数据实体
             * @param position   当前位置
             */
            @Override
            public void OnBannerClick(BannerBean bannerBean, int position) {
                Toast.makeText(MainActivity.this, bannerBean.getTitle()+position, Toast.LENGTH_SHORT).show();
            }
        });
        
        
        
         List<BannerBean> listBanner = new ArrayList();
//        for(int i=0;i<10;i++){
            BannerBean bb = new BannerBean();
            bb.setImg("https://pic0.iqiyipic.com/image/20220210/65/f1/v_165726475_m_601_m3_480_270.jpg");
            bb.setLink("https://www.iqiyi.com/v_t1r47dqqts.html");
            bb.setTitle("老九门之青山海棠");
            listBanner.add(bb);
//        }

        BannerBean bb0 = new BannerBean();
        bb0.setImg("https://pic9.iqiyipic.com/image/20230203/06/a7/v_151351479_m_601_m16_480_270.jpg");
        bb0.setLink("https://www.iqiyi.com/v_t1r47dqqts.html");
        bb0.setTitle("扫黑·决战");
        listBanner.add(bb0);

        BannerBean bb1 = new BannerBean();
        bb1.setImg("https://pic4.iqiyipic.com/image/20230313/0f/4a/a_100459089_m_601_m20_480_270.jpg");
        bb1.setLink("https://www.iqiyi.com/v_t1r47dqqts.html");
        bb1.setTitle("九霄寒夜暖");
        listBanner.add(bb1);

        BannerBean bb2 = new BannerBean();
        bb2.setImg("https://pic9.iqiyipic.com/image/20230315/a0/9a/v_171591295_m_601_m1_480_270.jpg");
        bb2.setLink("https://www.iqiyi.com/v_t1r47dqqts.html");
        bb2.setTitle("清明节放假");
        listBanner.add(bb2);

        BannerBean bb3 = new BannerBean();
        bb3.setImg("https://pic0.iqiyipic.com/lequ/common/lego/20230313/2741353a2d974ebea3b14c0180491a85.jpg");
        bb3.setLink("https://www.iqiyi.com/v_t1r47dqqts.html");
        bb3.setTitle("回响·定档0316");
        listBanner.add(bb3);

        BannerBean bb4 = new BannerBean();
        bb4.setImg("https://pic3.iqiyipic.com/lequ/common/lego/20230314/5a099f2b7b774d3c9814b2b09544060b.jpg");
        bb4.setLink("https://www.iqiyi.com/v_t1r47dqqts.html");
        bb4.setTitle("忠犬八公·院线定档");
        listBanner.add(bb4);




        banner.setBannerData(listBanner);
                    
                    
                    
