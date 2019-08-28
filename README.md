# DSA-LAB4
        #include<stdio.h>
        struct appliance
        {
            char name[20];
            long long int price,id;
            float discount;
        };
        struct appliance read()
        {
            struct appliance a;

                    printf("\nEnter Product name:");
                    scanf("%s",a.name);
                    printf("Enter Product id:");
                    scanf("%lld",&a.id);
                    printf("Enter Product price:");
                    scanf("%lld",&a.price);
                    printf("Enter Product discount:");
                    scanf("%f",&a.discount);

            return a;	
        }
        struct appliance write(struct appliance a)
            {

                    printf("\nProduct name:%s",a.name);
                    printf("\nProduct id:%lld",a.id);
                    printf("\nProduct price:%lld",a.price);
                    printf("\nProduct discount:%f%",a.discount);

            }
            main()
            {
                struct appliance x[10];
                int i,n;
                printf("Enter no. of products:");
                scanf("%d",&n);
                for(i=0;i<n;i++)
                {
                x[i]=read();
                }
                for(i=0;i<n;i++)
                {
                write(x[i]);
                }
            }



