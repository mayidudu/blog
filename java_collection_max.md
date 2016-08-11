java collection的max，min操作
```
@Test
    public void testCollection(){
        List<Integer> rssi_list = new ArrayList<Integer>();
        for (int i=0; i<10;i++)
            rssi_list.add(i+10);
        rssi_list.add(10);
        rssi_list.add(19);
        int max = Collections.max(rssi_list);
        Integer min = Collections.min(rssi_list);
        System.out.println(rssi_list);
        System.out.println("max:"+max);
        rssi_list.remove((Integer) max);
        rssi_list.remove((Integer)min);
        System.out.println(rssi_list);


    }
```
