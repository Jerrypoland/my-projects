def weight():
    w_type=input('''
    enter your type of weight. 
    press 'k' to convert in kilogram
    Press 'p' to convert in pound
    ''')
    w_type=w_type.lower()
    if w_type=='k':
        w = int(input('enter your weight in kg '))
        weight_in_pounds=w*2.205
        print(f'your {w} kilogram weight in pounds is {weight_in_pounds}')
        if weight_in_pounds>200:
            print('you are overweight')
        elif weight_in_pounds <200 and weight_in_pounds >100:
            print('your weight is average')
        else:
            print('you are so underweight')
    elif w_type=='p':
        w = int(input('enter your weight in pound '))
        weight_in_kilograms=w/2.205
        print(f'your {w} pound weight in kilogram is {weight_in_kilograms}')
    else:
        print('you have not defined the correct conversion weight')
        weight()

weight()
