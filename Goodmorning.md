# ATanalysisfunction varargout = VirtualInstruments(varargin)
% Begin initialization code - DO NOT EDIT
gui_Singleton = 1;
gui_State = struct('gui_Name',       mfilename, ...
                   'gui_Singleton',  gui_Singleton, ...
                   'gui_OpeningFcn', @VirtualInstruments_OpeningFcn, ...
                   'gui_OutputFcn',  @VirtualInstruments_OutputFcn, ...
                   'gui_LayoutFcn',  [] , ...
                   'gui_Callback',   []);
if nargin && ischar(varargin{1})
    gui_State.gui_Callback = str2func(varargin{1});
end

if nargout
    [varargout{1:nargout}] = gui_mainfcn(gui_State, varargin{:});
else
    gui_mainfcn(gui_State, varargin{:});
end
% End initialization code - DO NOT EDIT


% --- Executes just before VirtualInstruments is made visible.
function VirtualInstruments_OpeningFcn(hObject, eventdata, handles, varargin)
% This function has no output args, see OutputFcn.
% hObject    handle to figure
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
% varargin   command line arguments to VirtualInstruments (see VARARGIN)

% Choose default command line output for VirtualInstruments
handles.output = hObject;

    set(handles.edit7,'Value',0);
    set(handles.play,'Value',0);   
    
% Update handles structure
guidata(hObject, handles);

% UIWAIT makes VirtualInstruments wait for user response (see UIRESUME)
% uiwait(handles.figure1);


% --- Outputs from this function are returned to the command line.
function varargout = VirtualInstruments_OutputFcn(hObject, eventdata, handles) 
% varargout  cell array for returning output args (see VARARGOUT);
% hObject    handle to figure
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Get default command line output from handles structure
varargout{1} = handles.output;



function edit1_Callback(hObject, eventdata, handles)
% hObject    handle to edit1 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit1 as text
%        str2double(get(hObject,'String')) returns contents of edit1 as a double

    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.edit1 = NewVal;
    guidata(hObject,handles);


% --- Executes during object creation, after setting all properties.
function edit1_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit1 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function edit2_Callback(hObject, eventdata, handles)
% hObject    handle to edit2 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit2 as text
%        str2double(get(hObject,'String')) returns contents of edit2 as a double

    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.edit2 = NewVal;
    guidata(hObject,handles);


% --- Executes during object creation, after setting all properties.
function edit2_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit2 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function edit3_Callback(hObject, eventdata, handles)
% hObject    handle to edit3 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit3 as text
%        str2double(get(hObject,'String')) returns contents of edit3 as a double

    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.edit3 = NewVal;
    guidata(hObject,handles);


% --- Executes during object creation, after setting all properties.
function edit3_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit3 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function edit4_Callback(hObject, eventdata, handles)
% hObject    handle to edit4 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit4 as text
%        str2double(get(hObject,'String')) returns contents of edit4 as a double

    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.edit4 = NewVal;
    guidata(hObject,handles);


% --- Executes during object creation, after setting all properties.
function edit4_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit4 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function edit5_Callback(hObject, eventdata, handles)
% hObject    handle to edit5 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit5 as text
%        str2double(get(hObject,'String')) returns contents of edit5 as a double

    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.edit5 = NewVal;
    guidata(hObject,handles);


% --- Executes during object creation, after setting all properties.
function edit5_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit5 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end


% --- Executes on button press in pushbutton3.
function pushbutton3_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton3 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)   
    Signal.Amplitude  = handles.edit1;
    Signal.Frequency  = handles.edit2;
    Signal.Duration   = handles.edit3;
    
    N    = 4400;
    Fs   = 44000;                       % sampling frequency card
    df   = Fs/N;                        % freq res 10 Hz
    P    = round(Signal.Duration*Fs/N); % number of periods
    t    = [0:P*N-1]/Fs;
    in   = Signal.Amplitude * sin(2*pi*Signal.Frequency*t);
    ii   = 1;
    t0   = 0;

    timev = [];
    datat = [];

   
	while  get(handles.play,'Value') ~= 1;
        pause(0.05);
    end
    while  get(handles.edit7,'Value') ~= 1;
        fecha(ii)  = datenum(date);       
        temps(ii)  = datenum(rem(now,1));
        t          = datenum(datestr(clock));
        tstart     = tic;
        acc        = convertion(in,Fs);
        data       = in';

        windowlengthmin = abs(handles.tmax-handles.tmin);
        offsetmin       = abs((handles.tmax+handles.tmin)/2);
        randtimemin     = (rand(1)-0.5)*windowlengthmin+offsetmin;        
        telapsed        = toc(tstart);
        t               = addtodate(t, round(randtimemin*60+telapsed), 'second');  
        NextTime        = datestr(t);
        set(handles.edit12,'String',NextTime);
        pause(randtimemin*60);            
%         axes(handles.axes1);
%         plot(time,data);grid on
%         xlabel('Time (sec)')
%         ylabel('Acceleration')
        ii= ii+1;
        datat = [datat data];         
    end
    set(handles.edit7,'Value',0);
    set(handles.startbutton,'Value',0);    
    handles.accelerometer = datat;
%     handles.time          = time;
    handles.fecha         = fecha;  
    handles.temps         = temps;      
    
    guidata(hObject,handles);

    
    

% --- Executes on button press in pushbutton1.
function pushbutton1_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton1 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
    Signal.Amplitude  = handles.edit1;
    Signal.Frequency  = handles.edit2;
    Signal.Duration   = handles.edit3;
    Sweep.fmin        = handles.edit4;   
    Sweep.fmax        = handles.edit5;
    Sweep.NoFreqs     = handles.edit6;
    Sweep.t0          = 0;
    
    timev = [];
    datat = [];
    fechav = [];
    tempsv = [];
    
	windowlengthmin = abs(handles.tmax-handles.tmin);
	offsetmin       = abs((handles.tmax+handles.tmin)/2);
    
	while  get(handles.play,'Value') ~= 1;
        pause(0.05);
    end       
    
    while  get(handles.edit7,'Value') ~= 1;    
        [t,t0,acc,fecha,temps]    = sweep_frequency(handles,Signal, Sweep,windowlengthmin,offsetmin);
        Sweep.t0      = t0;
%         axes(handles.axes1);
%         plot(t,acc);grid on
%         xlabel('Time (sec)')
%         xlim([t(1,1) t0]);
%         ylabel('Acceleration')
                   
        timev  = [timev t];
        datat  = [datat acc];
        fechav = [fechav fecha];
        tempsv = [tempsv temps];
    end
    set(handles.edit7,'Value',0);
    set(handles.startbutton,'Value',0);   
    handles.accelerometer = datat;
%     handles.time          = timev;
    handles.fecha         = fechav;  
    handles.temps         = tempsv;  
    guidata(hObject,handles);


    

function edit6_Callback(hObject, eventdata, handles)
% hObject    handle to edit6 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit6 as text
%        str2double(get(hObject,'String')) returns contents of edit6 as a double
    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.edit6 = NewVal;
    guidata(hObject,handles);

% --- Executes during object creation, after setting all properties.
function edit6_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit6 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end


% --- Executes on button press in pushbutton5.
function pushbutton5_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton5 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
    set(handles.edit7, 'Value',1);
    set(handles.play, 'Value',0);    
    guidata(hObject,handles);


function edit7_Callback(hObject, eventdata, handles)
% hObject    handle to edit7 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit7 as text
%        str2double(get(hObject,'String')) returns contents of edit7 as a double
    set(handles.edit7,'Value',0);
    guidata(hObject,handles);

% --- Executes during object creation, after setting all properties.
function edit7_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit7 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end

%%
% --- Executes on button press in pushbutton6.
function pushbutton6_Callback(hObject, eventdata, handles)
% hObject    handle to pushbutton6 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
    Signal.Amplitude  = handles.edit1;
    Signal.Frequency  = handles.edit2;
    Signal.Duration   = handles.edit3;
    Sweep.Amin        = handles.edit4;   
    Sweep.Amax        = handles.edit5;
    Sweep.NoA         = handles.edit6;
	Sweep.t0          = 0;
    timev = [];
    datat = [];
    fechav = [];
    tempsv = [];

	windowlengthmin = abs(handles.tmax-handles.tmin);
	offsetmin       = abs((handles.tmax+handles.tmin)/2);
    
	while  get(handles.play,'Value') ~= 1;
        pause(0.05);
    end   
    while  get(handles.edit7,'Value') ~= 1;
        [t,t0,acc,fecha,temps]         = sweep_amplitude(handles,Signal, Sweep,windowlengthmin,offsetmin);
        Sweep.t0      = t0;
%         axes(handles.axes1);
%         plot(t,acc);grid on
%         xlabel('Time (sec)')
%         xlim([t(1,1) t0]);
%         ylabel('Acceleration')  
        
        timev = [timev t];
        datat = [datat acc];  
        fechav = [fechav fecha];
        tempsv = [tempsv temps];        
    end
    set(handles.edit7,'Value',0);
    set(handles.startbutton,'Value',0);  
    handles.accelerometer = datat;
    handles.time          = timev;
    handles.fecha         = fechav;  
    handles.temps         = tempsv;      
    guidata(hObject,handles);
   %% 
    
function edit11_Callback(hObject, eventdata, handles)
% hObject    handle to edit11 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit11 as text
%        str2double(get(hObject,'String')) returns contents of edit11 as a double


% --- Executes during object creation, after setting all properties.
function edit11_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit11 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function edit10_Callback(hObject, eventdata, handles)
% hObject    handle to edit10 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit10 as text
%        str2double(get(hObject,'String')) returns contents of edit10 as a double


% --- Executes during object creation, after setting all properties.
function edit10_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit10 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function edit9_Callback(hObject, eventdata, handles)
% hObject    handle to edit9 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit9 as text
%        str2double(get(hObject,'String')) returns contents of edit9 as a double


% --- Executes during object creation, after setting all properties.
function edit9_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit9 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end


% --------------------------------------------------------------------
function uipushtool5_ClickedCallback(hObject, eventdata, handles)
% hObject    handle to uipushtool5 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
 MA_step = 22; %resample accelerometer data 2kHz
 for ii  = 1:floor(size(handles.accelerometer,1)/MA_step)
        downsampleddata(ii,:) = mean(handles.accelerometer(1+ (ii-1)*(MA_step):ii*(MA_step),:));  
 end

[filename,pathname,filterIndex] = uiputfile('../*.xls','Select File to Save Data');
%figure;plot(handles.time,handles.accelerometer)
if isequal(filename,0) || isequal(pathname,0)
else
    xlswrite(strcat(pathname,filename),handles.temps','data','A1');
    xlswrite(strcat(pathname,filename),cellstr(datestr(handles.fecha)),'data','B1');
    xlswrite(strcat(pathname,filename),cellstr(datestr(handles.temps,13)),'data','C1');
%     xlswrite(strcat(pathname,filename),downsampleddata,'data','A4');
end



function edit12_Callback(hObject, eventdata, handles)
% hObject    handle to edit12 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of edit12 as text
%        str2double(get(hObject,'String')) returns contents of edit12 as a double


% --- Executes during object creation, after setting all properties.
function edit12_CreateFcn(hObject, eventdata, handles)
% hObject    handle to edit12 (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function tmin_Callback(hObject, eventdata, handles)
% hObject    handle to tmin (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of tmin as text
%        str2double(get(hObject,'String')) returns contents of tmin as a double
    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.tmin = NewVal;
    guidata(hObject,handles);

% --- Executes during object creation, after setting all properties.
function tmin_CreateFcn(hObject, eventdata, handles)
% hObject    handle to tmin (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function tmax_Callback(hObject, eventdata, handles)
% hObject    handle to tmax (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of tmax as text
%        str2double(get(hObject,'String')) returns contents of tmax as a double
    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.tmax = NewVal;
    guidata(hObject,handles);

% --- Executes during object creation, after setting all properties.
function tmax_CreateFcn(hObject, eventdata, handles)
% hObject    handle to tmax (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end


% --- Executes on button press in startbutton.
function startbutton_Callback(hObject, eventdata, handles)
% hObject    handle to startbutton (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
    set(handles.play, 'Value',1);    
    set(handles.edit7, 'Value',0);        
    guidata(hObject,handles);



function play_Callback(hObject, eventdata, handles)
% hObject    handle to play (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of play as text
%        str2double(get(hObject,'String')) returns contents of play as a double


% --- Executes during object creation, after setting all properties.
function play_CreateFcn(hObject, eventdata, handles)
% hObject    handle to play (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end


% --- Executes on button press in multisine.
function multisine_Callback(hObject, eventdata, handles)
% hObject    handle to multisine (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)
    load multisine40Hz200Hz
    Signal.Amplitude  = handles.edit1;
    Signal.Duration   = handles.edit3;
    
    % 1 Hz resolution
    Fs   = 44000;                       
    in   = repmat(Signal.Amplitude*u,1,round(Signal.Duration));
    ii   = 1;
    t0   = 0;

    timev = [];
    datat = [];
  
	while  get(handles.play,'Value') ~= 1;
        pause(0.05);
    end
    while  get(handles.edit7,'Value') ~= 1;
        if ii==1
            actualtime = datenum(datestr(now));
            waittime   = round(handles.waitstarttimehours*3600); 
            starttime  = addtodate(actualtime, waittime, 'second');              
            endtime    = addtodate(starttime, round(handles.stoptimehours*3600), 'second');            
            choice = questdlg(['Confirm timing loop sequence:: ' datestr(starttime) ' -- ' datestr(endtime)], ...
                'Stimuli loop sequence', ...
                'Yes','No','Yes');
            % Handle response
            switch choice
                case 'Yes'
                    set(handles.edit12,'String',datestr(starttime)); 
                    set(handles.showendtime,'String',datestr(endtime));
                    pause(waittime);
                case 'No'
                    set(handles.edit7,'Value',1); % stop execution
                    set(handles.play,'Value',0); % stop execution                    
            end
        end
        % Handle response
        switch choice
            case 'Yes'
                fecha(ii)  = datenum(date);       
                temps(ii)  = datenum(rem(now,1));
                t          = datenum(datestr(clock));
                tstart     = tic;
                acc        = convertion(in,Fs);
                data       = in';

                windowlengthmin = abs(handles.tmax-handles.tmin);
                offsetmin       = abs((handles.tmax+handles.tmin)/2);
                randtimemin     = (rand(1)-0.5)*windowlengthmin+offsetmin;        
                telapsed        = toc(tstart);
                t               = addtodate(t, round(randtimemin*60+telapsed), 'second');  
                NextTime        = datestr(t);

                if t >= endtime
                    set(handles.edit7,'Value',1); % stop execution
                else
                    set(handles.edit12,'String',NextTime);
                    pause(randtimemin*60);  
            %         axes(handles.axes1);
            %         plot(time,data);grid on
            %         xlabel('Time (sec)')
            %         ylabel('Acceleration')
                    ii= ii+1;
                    datat = [datat data];                 
%                     set(handles.edit7,'Value',0);
%                     set(handles.startbutton,'Value',0);    
                    handles.accelerometer = datat;
                %     handles.time          = time;
                    handles.fecha         = fecha;  
                    handles.temps         = temps;      
                end
                guidata(hObject,handles);                
        end
    end




function waitstarttimehours_Callback(hObject, eventdata, handles)
% hObject    handle to waitstarttimehours (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of waitstarttimehours as text
%        str2double(get(hObject,'String')) returns contents of waitstarttimehours as a double
    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.waitstarttimehours = NewVal;
    guidata(hObject,handles);

% --- Executes during object creation, after setting all properties.
function waitstarttimehours_CreateFcn(hObject, eventdata, handles)
% hObject    handle to waitstarttimehours (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function stoptime_Callback(hObject, eventdata, handles)
% hObject    handle to stoptime (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of stoptime as text
%        str2double(get(hObject,'String')) returns contents of stoptime as a double
    Val = get(hObject,'String');
    NewVal = str2double (Val);
    handles.stoptimehours = NewVal;
    guidata(hObject,handles);

% --- Executes during object creation, after setting all properties.
function stoptime_CreateFcn(hObject, eventdata, handles)
% hObject    handle to stoptime (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end



function showendtime_Callback(hObject, eventdata, handles)
% hObject    handle to showendtime (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    structure with handles and user data (see GUIDATA)

% Hints: get(hObject,'String') returns contents of showendtime as text
%        str2double(get(hObject,'String')) returns contents of showendtime as a double


% --- Executes during object creation, after setting all properties.
function showendtime_CreateFcn(hObject, eventdata, handles)
% hObject    handle to showendtime (see GCBO)
% eventdata  reserved - to be defined in a future version of MATLAB
% handles    empty - handles not created until after all CreateFcns called

% Hint: edit controls usually have a white background on Windows.
%       See ISPC and COMPUTER.
if ispc && isequal(get(hObject,'BackgroundColor'), get(0,'defaultUicontrolBackgroundColor'))
    set(hObject,'BackgroundColor','white');
end
