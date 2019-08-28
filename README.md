# DSA-LAB4
    #include<stdio.h>
    struct appliance
    {
      char name[20];
      long long int price,id;
      float discount;
    };
    void read()
    {
      struct appliance a[10];
      int n,i;
      printf("Enter number of products:");
      scanf("%d",&n);
        for(i=0;i<n;i++)
        {
          printf("\nEnter Product name:");
            scanf("%s",a[i].name);
          printf("Enter Product id:");
          scanf("%lld",&a[i].id);
          printf("Enter Product price:");
          scanf("%lld",&a[i].price);
          printf("Enter Product discount:");
          scanf("%f",&a[i].discount);
        }
    }
    void write()
      {
      int n,i;
      struct appliance a[10];	
        for(i=0;i<n;i++)
        {

          printf("\nProduct name:%s",a[i].name);
              printf("\nProduct id:%lld",a[i].id);
              printf("\nProduct price:%lld",a[i].price);
              printf("\nProduct discount:%f%",a[i].discount);
        }
      }
      main()
      {
        read();
        write();
      }

