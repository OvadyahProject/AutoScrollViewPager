# AutoScrollViewPager

### 最方便的可自动无限循环ViewPager插件, 完全适用于ViewPager

#### 使用方法
```
AutoBuilder.Builder(viewPager, list, new SimpleAutoListener<String>() {
            @Override
            public View initItemView(int position, String o) {
                TextView textView = new TextView(MainActivity.this);
                textView.setText(o);
                return textView;
            }
        })
                .setAutoLoop(true)
                .setAutomatic(true)
                .build();
```

>后续预计更新, 添加多样式ViewPager支持, 打造炫酷的切换动画