# Ari-code-Group-Menu-grouplink-jid-kickall-removecountry-662-kickadmins-add-
A simple WhatsApp bot to manage groups
╭━━〔 *Group Menu* 〕━━┈⊷
┃◈╭─────────────·๏
┃◈┃🔗 • grouplink
┃◈┃🔗 • jid
┃◈┃💣 • kickall
┃◈┃💣 • removecountry +662
┃◈┃👑 • kickadmins
┃◈┃➕ • add
┃◈┃➖ • remove
┃◈┃🦵 • kick
┃◈┃🔼 • promote 
┃◈┃🔽 • demote
┃◈┃♻️ • revoke
┃◈┃👋 • left
┃◈┃📄 • ginfo
┃◈┃🗑️ • delete 
┃◈┃✏️ • upgname
┃◈┃📝 • upgdesc
┃◈┃🔊 • groupunmute
┃◈┃🔇 • mute
┃◈┃🔈 • unmute
┃◈┃🔒 • lockgc
┃◈┃🔓 • unlockgc
┃◈┃🧾 • invite
┃◈┃🏷️ • tag
┃◈┃📢 • tagall
┃◈┃📢 • broadcast
┃◈┃❤️ • ship
┃◈┃🧾 • shapar
┃◈┃🫣 • compatibility
┃◈┃🤔 • roast
┃◈┃🥰 • compliment
┃◈┃😍 • lovetest
┃◈┃🙂‍↔️ • nikal
┃◈└───────────┈⊷
╰──────────────┈⊷
> * ❤️Group All Command Working Smoothly All Error Fixed Antilink Working*
> * https://github.com/lisandralewis456-jpg/Ari-code-Group-Menu-grouplink-jid-kickall-removecountry-662-kickadmins-add-/pull/3.patch 
loyment status for #{@payload['id']} is #{@payload
start_deployment(pull_request)
  user = pull_request['user']['login']
  payload = JSON.generate(:environment => 'production', :deploy_user => user)
  @client.create_deployment(pull_request['head']['repo']['full_name'], pull_request['head']['sha'], {:payload => payload, :description => "Deploying my sweet branch"})
>
endpost '/event_handler' do
  @payload = JSON.parse(params[:payload])

  case request.env['HTTP_X_GITHUB_EVENT']
  when "pull_request"
    if @payload["action"] == "closed" && @payload["pull_request"]["merged"]
      puts "A pull request was merged! A deployment should start now..."
    end
  end
end
send this information to your chat room, monitor, pager, etc.
  puts "Processing '#{@payload['description']}' for #{payload['deploy_user']} to #{payload['environment']}"
  sleep 2 # simulate work
  @client.create_deployment_status("repos/#{@payload['repository']['full_name']}/deployments/#{@payload['id']}", 'pending')
  sleep 2 # simulate work
  @client.create_deployment_status("repos/#{@payload['repository']['full_name']}/deployments/#{@payload['id']}", 'success')
end
